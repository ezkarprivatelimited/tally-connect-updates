# Tally Connect Updates

This repository hosts the official release distributions and update configurations for **Tally Connect**. It acts as the remote endpoint for checking and downloading the latest application updates.

## Current Release

- **Latest Version:** `v1.0.0`
- **Release Notes:** Initial release of Tally Connect with basic features and improvements.

### 📥 Download

You can download the latest version installer directly below:
[**Download TallyConnect_Setup.exe (v1.0.0)**](https://raw.githubusercontent.com/ezkarprivatelimited/tally-connect-updates/main/releases/download/v1.0.0/TallyConnect_Setup.exe)

---

## ⚙️ How the Updater Works

The application checks for updates by fetching the [`version.json`](./version.json) file from this repository. 

The file contains the following metadata:
- **`version`**: The latest available semantic version number.
- **`url`**: The direct download URL for the respective installer/update package.
- **`notes`**: The changelog or release notes indicating what's new.

When the remote version is greater than the locally installed version, the application will prompt the user to download from the provided `url`.

## 📁 Repository Structure

```text
.
├── releases/
│   └── downloads/
│       └── v1.0.0/           # Contains actual asset files if hosted directly in repo
├── version.json              # The metadata file polled by the application updater
└── README.md                 # This documentation file
```