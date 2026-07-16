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
3. In Gear Lever, click on **Antigravity 2** in your list, go to the **Update Management** section, and select **GitHub** as the update source.
4. Fill in the fields exactly as follows:
   - **Repository (owner/repo)**: 
     ```text
     PrudviTeja99/antigravity-appimage-builder
     ```
   - **Application file name** (or **Asset name**): 
     ```text
     Antigravity_2-*-x86_64.AppImage
     ```
     *(The asterisk `*` acts as a wildcard that allows Gear Lever to check and match future version releases).*
