# Antigravity 2 AppImage Builder

This repository contains an automated GitHub Actions workflow to build and release portable AppImage versions of Google Antigravity 2 for Linux (x86_64).

## Setup Instructions

To push this workflow to your remote GitHub repository, open your terminal and follow these steps:

### 1. Navigate to the project directory
```bash
cd /home/teja/.gemini/antigravity/scratch/antigravity-appimage-builder
```

### 2. Initialize Git
```bash
git init
```

### 3. Stage the files
```bash
git add .
```

### 4. Create your first commit
```bash
git commit -m "Initial commit: Add AppImage build workflow"
```

### 5. Rename default branch to `main`
```bash
git branch -M main
```

### 6. Create a repository on GitHub
1. Go to your GitHub dashboard and click **New Repository**.
2. Name the repository (e.g. `antigravity-appimage-builder`).
3. Keep it empty (do **not** initialize it with a README, gitignore, or license).
4. Copy the remote URL (e.g. `git@github.com:YOUR_USERNAME/antigravity-appimage-builder.git` or `https://github.com/YOUR_USERNAME/antigravity-appimage-builder.git`).

### 7. Link to the Remote Repository
Replace `YOUR_REMOTE_URL` with the URL you copied:
```bash
git remote add origin YOUR_REMOTE_URL
```

### 8. Push to GitHub
```bash
git push -u origin main
```

---

## Triggering the Build

Once pushed, you can run the builder in two ways:
1. **Automatically (Scheduled)**: The workflow runs automatically every day at midnight to search the Google website for newer releases. If a new version exists, it will automatically package and release it.
2. **Manually**: 
   * Navigate to the **Actions** tab of your GitHub repository.
   * Select the **Build Antigravity 2 AppImage** workflow.
   * Click **Run workflow** and optionally provide a custom download URL or version tag override.
