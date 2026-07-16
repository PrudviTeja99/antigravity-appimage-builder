# Google Antigravity 2 AppImage Builder

This repository contains an automated GitHub Actions workflow to build and release portable Linux AppImages for **Google Antigravity 2**.

## 🚀 Features

- **Automated Daily Updates**: Checks for new releases on the Google Antigravity website every day. If a new version is found, it automatically builds and releases the AppImage.
- **Portability**: Compiles the AppImage on `ubuntu-latest` for wide compatibility across modern Linux distributions.

## 📦 How to Download and Run

1. Go to the **Releases** tab of this repository.
2. Download the latest `.AppImage` file.
3. Make the file executable in your terminal:
   ```bash
   chmod +x Antigravity_2-*.AppImage
   ```
4. Run the application:
   ```bash
   ./Antigravity_2-*.AppImage
   ```

### ⚙️ Desktop Integration & Auto-Updates (Recommended)

To integrate the application into your system menus and enable automatic background updates:
1. Install [Gear Lever](https://github.com/mijorus/gearlever) (available on Flathub).
2. Open Gear Lever and drag-and-drop the downloaded `.AppImage` file to integrate it.
3. In Gear Lever, configure the Update Source to **GitHub** and paste the following release URL:
   ```text
   https://github.com/PrudviTeja99/antigravity-appimage-builder/releases/download/v*/Antigravity_2-*-x86_64.AppImage
   ```
   *(Gear Lever will check this link in the background and automatically update your installation whenever a new version is published here).*
