# Installation

Dolphin {anty} is a desktop application available for Windows, macOS, and Linux.

## System Requirements

| OS | Minimum Requirements |
|----|---------------------|
| Windows | Windows 10 or later, 64-bit |
| macOS | macOS 10.14 (Mojave) or later |
| Linux | Ubuntu 18.04+, Debian, or compatible |

## Download

Visit the [official download page](https://dolphin-anty.com/) and click the download button for your platform:

- **Windows**: `.exe` installer
- **macOS**: `.dmg` disk image  
- **Linux**: `.AppImage` or `.deb` package

## Installation Steps

### Windows

1. Run the downloaded `.exe` file
2. Follow the installation wizard
3. Launch Dolphin {anty} from the Start menu or desktop shortcut

### macOS

1. Open the downloaded `.dmg` file
2. Drag **Dolphin {anty}** to your Applications folder
3. Open from Applications — if macOS blocks it, go to **System Preferences → Security & Privacy** and click **Open Anyway**

### Linux

**AppImage:**
```bash
chmod +x dolphin-anty.AppImage
./dolphin-anty.AppImage
```

**Debian/Ubuntu (.deb):**
```bash
sudo dpkg -i dolphin-anty.deb
sudo apt-get install -f  # fix dependencies if needed
```

## First Launch

After installation, launch the application and log in with your Dolphin {anty} account. If you don't have an account yet, [create one for free](https://dolphin-anty.com/).

## Updating

Dolphin {anty} will notify you when updates are available. You can also check for updates manually within the application settings.

## Uninstalling

- **Windows**: Use **Add or Remove Programs** in Windows Settings
- **macOS**: Drag the app from Applications to Trash
- **Linux**: `sudo dpkg -r dolphin-anty` or delete the AppImage
