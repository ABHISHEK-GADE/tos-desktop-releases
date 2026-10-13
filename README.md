# Tips On Stream Desktop Releases

<div align="center">

[![Windows 10 / 11](https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011%20(x64)-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/latest)
[![Latest Release](https://img.shields.io/badge/Latest%20Version-v1.0.4-FA8F38?style=for-the-badge&logo=rocket&logoColor=white)](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/latest)
[![OBS Studio](https://img.shields.io/badge/OBS%20WebSocket-v5.0%20Compatible-27B070?style=for-the-badge&logo=obsstudio&logoColor=white)](https://obsproject.com/)
[![Built For Streamers](https://img.shields.io/badge/Built%20For-Live%20Streamers-3A6DE4?style=for-the-badge&logo=youtube&logoColor=white)](https://tipsonstream.in)

### High-performance, broadcast-safe Windows companion software for Indian live streamers.
#### Real-time OBS integration, local multi-platform chatbots, instant alert replays, and zero-interruption background updates.

[**⬇️ Download Latest Installer (v1.0.4)**](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/download/v1.0.4/Tips-On-Stream-Companion-Setup-1.0.4.exe) • [**🌐 Web Platform**](https://tipsonstream.in) • [**📖 Documentation**](https://tipsonstream.in/guides)

</div>

---

## ⚡ Quick Download & Current Production Release

| Component | Specification | Direct Download |
| :--- | :--- | :--- |
| **Latest Version** | `v1.0.4` (Production Milestone) | [**Download Setup .exe**](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/download/v1.0.4/Tips-On-Stream-Companion-Setup-1.0.4.exe) |
| **Artifact Name** | `Tips-On-Stream-Companion-Setup-1.0.4.exe` | *(Windows 64-bit NSIS Installer)* |
| **File Size** | `83.74 MB` (87,807,404 bytes) | [**View Release Assets**](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/tag/v1.0.4) |
| **Auto-Update Feed** | Enabled via `latest.yml` delta blockmap | Automatic silent in-place upgrades |
| **System Compatibility** | Windows 10 (Build 19041+) / Windows 11 (x64) | OBS Studio v28.0+ |

---

## 📋 Release Changelog Registry (Last 5 Versions)

All official client releases are cataloged below in chronological order (newest at the top, oldest at the bottom).

```
v1.0.4 (Latest)  ──►  v1.0.3  ──►  v1.0.2  ──►  v1.0.1  ──►  v1.0.0 (Genesis)
```

---

### 🚀 [v1.0.4] - 2026-10-13 (Latest Production Release)
> **Authentic Branding Architecture & Windows 11 Smart App Control Hardening**

[📦 Release Assets & Download](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/tag/v1.0.4)

#### ✨ Highlights & New Capabilities
- **Crisp, Unwrapped Brand Icons:** Completely eliminated artificial container boxes, dark tile backgrounds, outer borders, extra padding, and squircle clipping shells across the entire desktop companion:
  - **Frameless Titlebar Header:** Replaced padded wrapper with pixel-accurate `object-contain` rendering for a flush silhouette on dark streaming workspaces.
  - **Sign-In & Auth Screen:** Removed boxy clipping layers; the brand mark now displays with natural transparency and razor-sharp contrast.
  - **About & Legal Store Card:** Unwrapped nested background tile for a modern, native Windows 11 look.
  - **Electron Loopback Server Landing Page (`/auth/callback`):** Removed container shadows and borders, standardizing on a clean, responsive logo presentation.
- **In-Memory NSIS PE Uninstaller Extraction:** Re-engineered the NSIS packaging pipeline to perform in-memory PE uninstaller binary extraction (`UninstallerReader.exec`), preventing Windows 11 Smart App Control execution blocks during packaging and uninstallation routines.
- **High-DPI Multi-Resolution Smoothing:** Calibrated SVG and multi-resolution mipmap icons (16px to 256px) to eliminate sub-pixel fuzziness across 100%, 125%, 150%, and 200% Windows display scaling settings.

#### 🛡️ Stability & Security
- Passed 100% pre-flight test suites (29 test files, 282 automated tests passing).
- Verified zero memory leaks during long-running background OBS listeners.

#### 🔒 Binary Verification
- **Artifact:** `Tips-On-Stream-Companion-Setup-1.0.4.exe`
- **File Size:** `87,807,404 bytes` (~83.74 MB)
- **SHA512 Checksum:**
  ```text
  7361D562FD529A9D319E7A7FF3353AF419D900BC126543C20BB95ACA98196BA5DDEE8808DD1627841132C1E7BA5EFF6FCF86C9C7EDB68248EA3C3013043C1371
  ```

---

### ⚡ [v1.0.3] - 2026-10-13
> **Seamless 1-Click Silent Auto-Updates & Zero-Prompt Restart**

[📦 Release Assets & Download](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/tag/v1.0.3)

#### ✨ Highlights & New Capabilities
- **Zero-Prompt Silent Update Execution:** Upgraded the `autoUpdater.quitAndInstall` engine with verified silent parameters (`isSilent: true, isForceRunAfter: true`). When an update is ready, clicking "Restart & Apply Update" instantly installs the update in the background with `/S` and `--force-run` flags.
- **Skipped Interactive Setup Wizard on Updates:** Existing installations no longer trigger the multi-page NSIS setup wizard (License Agreement, directory selector, and completion screens) when upgrading.
- **1-2 Second Hot Restart:** Streamers experience an instant in-place refresh directly into the newly patched companion version.
- **Process Lock Contention Prevention:** Direct download fallback installer spawns with silent flags (`["/S", "--updated", "--force-run"]`) and immediately releases process file locks via `app.exit(0)`, preventing "Application is currently running" lockup dialogs.
- **Active Broadcast Protection:** Automatic detection via OBS WebSocket 4455 ensures updates remain queued and deferred whenever live broadcasting or recording is detected.

#### 🔒 Binary Verification
- **Artifact:** `Tips-On-Stream-Companion-Setup-1.0.3.exe`
- **File Size:** `87,806,377 bytes` (~83.74 MB)
- **SHA512 Checksum:**
  ```text
  BgXYfv4y/g1Za05AwPdYwFWu+EZOfPbBVXJd1mC6uaoGWg3ILkOkVkG86EqKzK6UFHiRcj7PvUEh7lVTKXmTpg==
  ```

---

### 🔄 [v1.0.2] - 2026-10-13
> **Resilient Direct Downloader Engine & Real-Time Progress Streaming**

[📦 Release Assets & Download](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/tag/v1.0.2)

#### ✨ Highlights & New Capabilities
- **Direct GitHub Release Fallback Downloader:** Built a direct streaming downloader that resolves release binary assets directly from the GitHub Releases API whenever standard CDN feed manifests encounter network issues.
- **Real-Time Transfer Metrics:** Displays live download speed in MB/s, transferred megabytes vs total bytes, and completion percentage.
- **High-Visibility Download Progress Bar:** Integrated animated Brand Orange (`#FA8F38`) / Brand Glow (`#FFBA66`) progress bars into the frameless titlebar header, Settings tab, and global notification banner.
- **1-Click Update Triggers:** Added visible, one-click update actions directly in the companion viewport so streamers can trigger downloads at their convenience.
- **Windows 11 Action Center Notification Branding:** Configured registry `AppUserModelId` and native shortcut metadata targeting `$appExe` at icon index 0, eliminating generic placeholder icons on Windows desktop toast notifications.

#### 🔒 Binary Verification
- **Artifact:** `Tips-On-Stream-Companion-Setup-1.0.2.exe`
- **File Size:** `87,806,499 bytes` (~83.74 MB)
- **SHA512 Checksum:**
  ```text
  0BCA54F9B54EAF3AAE38A1F1EB493B133AC571DF706CE3D2F60E78EAF8AE4A5CC97848994BE96A3036F4C7F431AA5998132D59684C1B33A2AECF5DFCC4FE99B0
  ```

---

### 🌐 [v1.0.1] - 2026-10-12
> **Segregated Public CDN Distribution Pipeline & Delta Blockmaps**

[📦 Release Assets & Download](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/tag/v1.0.1)

#### ✨ Highlights & New Capabilities
- **Decoupled Public CDN Pipeline:** Shifted auto-update and installer distribution to this dedicated public release repository (`tos-desktop-releases`). Streamers receive fast, unauthenticated CDN downloads without exposing private source code or requiring private access tokens.
- **SHA512 Delta Blockmap Patching:** Introduced `.blockmap` binary indexing for lightning-fast differential downloads, saving streamer bandwidth during frequent updates.
- **Broadcast-Safe Auto-Update Engine:** Initial implementation of the OBS Stream Guard, deferring updates whenever live streaming is in progress.
- **1-Click Titlebar & Tray Controls:** Added update status badges and restart actions directly to the companion titlebar and system tray menu.

#### 🔒 Binary Verification
- **Artifact:** `Tips On Stream Companion Setup 1.0.1.exe`
- **File Size:** `~87.7 MB`
- **Manifest:** `latest.yml` verified

---

### 🌟 [v1.0.0] - 2026-10-12 (Genesis Milestone)
> **The Official Genesis Production Release for Windows**

[📦 Release Assets & Download](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/tag/v1.0.0)

#### ✨ Highlights & New Capabilities
- **Low-Latency OBS WebSocket Integration:** Native local loopback connection on port `4455` (OBS WebSocket v5) for instant browser-source alert injection and stream state monitoring.
- **Multi-Platform Live Chatbots:** Local engine running lightweight chatbots for YouTube, Twitch, and Kick to automate chat announcements and tipping links without hitting cloud quota bottlenecks.
- **Streamer Workstation Dock:** Built-in floating dock with instant alert replays, thank-you shortcuts, real-time crowdfunding goal progress bars, and missed alert backlog management.
- **Professional Windows NSIS Setup Wizard:** Custom setup wizard including EULA terms, custom installation directory selector, Start Menu & desktop shortcut creation, and launch toggle.
- **Frameless Dark-Mode Fluent UI:** Modern Windows 11 interface with custom window controls (minimize, maximize, close), snap layout support, and minimize-to-tray background execution.
- **Zero-Load Architecture:** Bundles all interface assets locally; connects directly to backend services over secure TLS/WebSockets with zero server polling overhead.

#### 🔒 Binary Verification
- **Artifact:** `Tips On Stream Companion Setup 1.0.0.exe`
- **File Size:** `~87.7 MB`
- **Platform:** Windows 10 / Windows 11 (x64)

---

## 🛠️ System Requirements & Compatibility

| Requirement | Minimum | Recommended |
| :--- | :--- | :--- |
| **Operating System** | Windows 10 (Build 19041+) 64-bit | Windows 11 (Build 22000+) 64-bit |
| **Processor** | Intel Core i3 or AMD Ryzen 3 (x64) | Intel Core i5 or AMD Ryzen 5+ |
| **Memory (RAM)** | 4 GB | 8 GB or higher |
| **Storage** | 300 MB free disk space | SSD storage recommended |
| **Streaming Software** | OBS Studio v28.0+ *(with WebSocket enabled)* | OBS Studio v30.0+ |
| **Internet** | Stable broadband connection | Low-latency fiber connection |

---

## 📥 Installation & Setup Guide

1. **Download Installer:** Grab the latest `Tips-On-Stream-Companion-Setup-x.x.x.exe` from the [Releases](https://github.com/ABHISHEK-GADE/tos-desktop-releases/releases/latest) section.
2. **Run Setup:** Double-click the installer, review the Terms of Service, choose your preferred destination directory, and complete setup.
3. **Connect Your Account:** Click **Sign In with Tips On Stream** to sync with your creator profile via fast local loopback authentication (`127.0.0.1:57891`).
4. **Pair with OBS Studio:** Open OBS Studio. The companion connects locally over WebSocket port `4455` automatically.
5. **Start Streaming:** Enjoy real-time tip alerts, TTS voice readouts, chat automation, and floating workstation controls!

---

## 🔐 How to Verify Checksums

To verify the integrity of any downloaded installer binary against the official release hashes, run the following command in Windows PowerShell:

```powershell
Get-FileHash -Path ".\Tips-On-Stream-Companion-Setup-1.0.4.exe" -Algorithm SHA512 | Format-List
```

Compare the resulting hash with the SHA512 string documented under the corresponding release above.

---

<div align="center">

**Tips On Stream** • Built with passion for creators by **Twice Scale**  
[Official Website](https://tipsonstream.in) • [Creator Dashboard](https://tipsonstream.in/dashboard) • [Support & Guides](https://tipsonstream.in/guides)

</div>
