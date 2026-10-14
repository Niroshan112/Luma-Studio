<div align="center">

# Luma Creative Studio POS

### A simple, reliable point-of-sale desk for photo framing & printing

[![Windows](https://img.shields.io/badge/Platform-Windows-2563eb?style=for-the-badge&logo=windows)](https://github.com/Niroshan112/Luma-Studio/releases)
[![Electron](https://img.shields.io/badge/Desktop-Electron-47848f?style=for-the-badge&logo=electron)](https://www.electronjs.org/)
[![React](https://img.shields.io/badge/UI-React-149eca?style=for-the-badge&logo=react)](https://react.dev/)

**Made for Luma Creative Studio · Balabowa, Dewalapola, Sri Lanka**

</div>

---

## ✨ About

Luma POS brings daily shop tasks into one desktop app. Create sales, manage
frame prices and stock, keep customer details, follow framing orders, and print
receipts—all in one place, with prices in Sri Lankan Rupees.

## 🧰 What it can do

| Area | Includes |
| --- | --- |
| **Sales register** | Browse and search the catalog, add items to a cart, and record payments |
| **Frames & prices** | Manage frame sizes, thicknesses, selling prices, and stock |
| **Customers** | Keep customer names, phone numbers, and order history together |
| **Orders** | Track framing work and pickup progress |
| **Receipts** | Print customer bills on supported receipt paper or A4 |
| **Reports** | Review sales totals and past transactions |
| **Backups** | Manage local data and configure Google Drive backup |
| **Updates** | Check for a published release and update from the login screen |

> **Designed for shop use:** sales data is stored locally on the POS computer.
> Keep regular backups, and use a trusted, access-controlled Windows account.

## 🚀 Install the POS

Download the latest Windows installer from
[**GitHub Releases**](https://github.com/Niroshan112/Luma-Studio/releases), run
it, and follow the setup prompts.

## 🧑‍💻 Run from source

Requirements: Windows, Node.js, and npm.

```powershell
npm install
npm run dev
```

To create a Windows installer:

```powershell
npm run package:install
```

The versioned installer and update metadata are created in `release/`:

```text
Luma-POS-<version>-x64.exe
latest.yml
```

## 🔄 Publish an update

Updates are hosted in the public
[`Niroshan112/Luma-Studio` GitHub repository](https://github.com/Niroshan112/Luma-Studio).
When an update is available, **Update POS** appears on the login screen. Click
it to download and install the update.

### First release setup

1. Build this project's installer with `npm run package:install`.
2. Create a GitHub Release with a tag that matches the app version, such as
   `v1.0.2`.
3. Upload **both** `Luma-POS-1.0.2-x64.exe` and `latest.yml` from `release/`.
4. Publish the release.
5. Install this updater-enabled installer **once** on each POS computer. Older
   installations need this one-time manual install before they can update
   themselves.

### Every release after that

1. Increase the app version in `package.json` (for example, `1.0.2` to
   `1.0.3`).
2. Run `npm run package:install`.
3. Draft a GitHub Release using the matching tag (for example `v1.0.3`).
4. Upload the new version's `.exe` and `latest.yml` from `release/`, then
   publish.

POS computers check for updates when the app starts. A newer release will show
**Update POS** on the login screen; staff can choose when to download and
install it.

## 🛠️ Built with

- [React](https://react.dev/) and [Vite](https://vite.dev/) for the POS interface
- [Electron](https://www.electronjs.org/) for the Windows desktop app
- [Dexie](https://dexie.org/) for local IndexedDB storage
- [electron-updater](https://www.electron.build/auto-update) for GitHub release updates

---

<div align="center">

**Luma Creative Studio** · 45/D Balabowa, Dewalapola · Sri Lanka

</div>
