# Automation & API

Dolphin {anty} supports multiple automation approaches — from no-code scenario builders to full programmatic control via REST API and browser automation frameworks.

## Automation Options

| Method | Skill Level | Use Case |
|--------|-------------|----------|
| Scenario Builder | No code | Account farming, form filling |
| Local API | Developer | Control profiles programmatically |
| Remote API | Developer | Manage accounts from external services |
| Selenium | Developer | Browser automation scripts |
| Puppeteer | Developer | Node.js browser automation |
| Playwright | Developer | Cross-browser automation |

## Scenario Builder

The built-in **Script Builder** lets you create automated workflows without writing code:

1. Go to **Script Builder** in the main menu
2. Create a new scenario
3. Add actions: navigate, click, type, wait, etc.
4. Attach the scenario to profiles
5. Run via **Mass Actions → Run Script**

Available on Windows, Linux, and macOS. Suitable for:
- Account farming sequences
- Form submission workflows
- Data collection tasks

## Local API

The Local API runs on your machine and lets you control browser profiles programmatically.

### Starting a Profile

```bash
GET http://localhost:3001/v1.0/browser_profiles/{profile_id}/start
```

Response:
```json
{
  "automation": {
    "port": 9222,
    "wsEndpoint": "ws://127.0.0.1:9222/devtools/browser/..."
  }
}
```

### Stopping a Profile

```bash
GET http://localhost:3001/v1.0/browser_profiles/{profile_id}/stop
```

### API Port

The local API listens on port `3001` by default. Enable it in **Settings → API**.

## Remote API

The Remote API lets external services control Dolphin {anty} over the internet.

### Authentication

All remote API requests require a Bearer token:

```bash
Authorization: Bearer YOUR_API_TOKEN
```

Generate your token in **Personal Cabinet → API**.

### Base URL

```
https://dolphin-anty-api.com
```

### Common Endpoints

```bash
# List all profiles
GET /browser_profiles

# Create a profile
POST /browser_profiles

# Get profile details
GET /browser_profiles/{id}

# Delete a profile
DELETE /browser_profiles/{id}
```

## Selenium Integration

Connect Selenium to a running Dolphin {anty} profile:

```python
from selenium import webdriver
from selenium.webdriver.chrome.options import Options
import requests

# Start the profile via Local API
response = requests.get('http://localhost:3001/v1.0/browser_profiles/{PROFILE_ID}/start')
data = response.json()
ws_endpoint = data['automation']['wsEndpoint']
port = data['automation']['port']

# Connect Selenium
options = Options()
options.add_experimental_option("debuggerAddress", f"127.0.0.1:{port}")
driver = webdriver.Chrome(options=options)

# Now use driver normally
driver.get("https://example.com")
```

## Puppeteer Integration

```javascript
const puppeteer = require('puppeteer-core');
const fetch = require('node-fetch');

async function main() {
  // Start profile
  const res = await fetch('http://localhost:3001/v1.0/browser_profiles/PROFILE_ID/start');
  const { automation } = await res.json();

  // Connect to profile
  const browser = await puppeteer.connect({
    browserWSEndpoint: automation.wsEndpoint,
    defaultViewport: null,
  });

  const page = await browser.newPage();
  await page.goto('https://example.com');
}

main();
```

## Playwright Integration

```python
from playwright.sync_api import sync_playwright
import requests

# Start the profile
response = requests.get('http://localhost:3001/v1.0/browser_profiles/{PROFILE_ID}/start')
ws_endpoint = response.json()['automation']['wsEndpoint']

with sync_playwright() as p:
    browser = p.chromium.connect_over_cdp(ws_endpoint)
    page = browser.new_page()
    page.goto('https://example.com')
```

## API Documentation

Full API reference is available at the [official documentation](https://help.dolphin-anty.com/en/).
