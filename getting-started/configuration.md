# Configuration

Initial setup and key settings for Dolphin {anty}.

## Account Settings

After logging in, visit your **Personal Cabinet** to configure:

- **Plan**: View your current subscription and upgrade if needed
- **Team members**: Add users to your workspace (Base plan and above)
- **API tokens**: Generate tokens for automation

## Application Settings

Access settings from the main menu (bottom-left area of the interface):

### General

- **Language**: Choose your interface language (English, Russian, Ukrainian, Spanish, Portuguese, Vietnamese)
- **Theme**: Switch between light and dark mode
- **Auto-update**: Enable/disable automatic updates

### Cloud Synchronization

Cloud sync is enabled by default. Your browser profiles, cookies, and settings sync across all devices logged into the same account.

To **disable cloud sync** (keep profiles local only):
1. Open Settings
2. Go to **Synchronization**
3. Toggle **Local sync** — profiles stay on your device only

### Extensions

Extensions are managed globally, not per-profile. To add an extension:

1. Go to **Main Menu → Extensions**
2. Install extensions here — they'll be available across all profiles

> **Important**: Do not install extensions from inside individual browser profiles. Always use the main menu extension manager.

### Proxies

Configure your proxy list once and reuse across profiles:

1. Go to **Proxies** in the sidebar
2. Add proxies (HTTP, HTTPS, SOCKS4, SOCKS5)
3. When creating a profile, select a saved proxy from the list

See [Proxy Management](../features/proxies.md) for detailed instructions.

## Team Configuration

If you have a Base plan or higher, you can add team members:

1. Go to **Team** in your Personal Cabinet
2. Click **Add User** and enter their email
3. Assign roles: **Admin**, **User**, or custom permissions
4. Share specific profile folders with team members

## API Configuration

For automation, generate an API token:

1. Go to **Personal Cabinet → API**
2. Click **Generate Token**
3. Use the token in your automation scripts

See [Automation & API](../features/automation.md) for usage examples.
