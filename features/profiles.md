# Browser Profiles

Browser profiles are the core of Dolphin {anty}. Each profile is a fully isolated browser environment with its own cookies, local storage, cache, and fingerprint.

## Creating a Profile

1. Click **Create Profile** in the main toolbar
2. Enter a **Profile Name**
3. (Optional) Select or add a **Proxy**
4. (Optional) Configure fingerprint settings — defaults are recommended
5. Add **Tags**, **Status**, or **Notes** for organization
6. Click **Save**

## Profile Settings

### Basic Settings

| Setting | Description |
|---------|-------------|
| Name | Identifier for the profile |
| Proxy | Assign an HTTP/HTTPS/SOCKS proxy |
| Tags | Color-coded labels for categorization |
| Status | Current state (e.g., Farming, New, Ready to Run) |
| Notes | Free-text notes visible to team members |
| Folder | Organize profiles into folders |

### Fingerprint Settings

Leave these at their defaults unless you have a specific reason to change them. See [Fingerprint Management](fingerprints.md) for details.

## Managing Profiles

### Organizing

Use **folders** to group related profiles (e.g., by client, platform, or campaign). Move profiles between folders by right-clicking or using the context menu.

Use **tags** for quick visual filtering — color-code by account type, status, or ownership.

### Mass Actions

Select multiple profiles using checkboxes, then apply bulk operations:

- **Start** — launch all selected profiles
- **Stop** — close all selected profiles
- **Run Script** — execute an automation script
- **Export Cookies** — save cookie data
- **Assign Tags** — bulk-label profiles
- **Transfer** — move profiles to a team member
- **Move to Folder** — reorganize
- **Delete** — remove profiles

### Search and Filter

Use the search bar to find profiles by name. Filter by tag, status, folder, or proxy type from the sidebar.

## Profile Limits by Plan

| Plan | Profile Limit |
|------|--------------|
| Free | 5 |
| Starter | 60 |
| Base | 100 |
| Team | 300 |
| Enterprise | Unlimited |
| Custom | Unlimited |

## Sharing Profiles

On Base plan and above, you can share profiles or folders with team members. Assign granular permissions: view only, edit, or full control.

## Exporting and Importing Cookies

To transfer cookies from an existing account into a profile:

1. Open the profile
2. Go to **Profile Settings → Cookies**
3. Paste cookie data in JSON format
4. Save and restart the profile
