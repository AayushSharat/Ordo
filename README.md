# Ordo

A fast, featherweight keyboard launcher for Windows. Press **Ctrl+Space**, type, and
instantly launch apps, find files, do quick math, search the web, open Windows Settings,
or run commands — all from one bar.

Built in native Rust (no Electron, no web runtime), so it stays tiny and instant:
~2–4 MB idle RAM, 0% idle CPU, a ~1.5 MB binary, and results in well under a frame.

### 🌐 Website & demo video → **[ordo-website-three.vercel.app](https://ordo-website-three.vercel.app)**

## Download

**[⬇ Download the latest version](https://github.com/AayushSharat/Ordo/releases/latest)**

- **Installer** (`OrdoSetup-x.y.z.exe`) — per-user, no admin needed. Recommended.
- **Portable** (`Ordo-x.y.z-portable.zip`) — unzip and run `ordo.exe`.

> **SmartScreen note:** Ordo isn't code-signed yet, so Windows may show *"Windows
> protected your PC."* Click **More info → Run anyway**. (Code signing is planned.)

## Features

- **App launch** — fuzzy-search everything in your Start Menu, including Store apps.
- **File search** — instant, Everything-style filename search. Indexes Desktop, Documents,
  Downloads, Pictures, Videos & Music by default; add any folder by typing **`add folder`**.
- **Calculator** — type `2+2*8`, `sqrt(144)`, `0xff+1`; Enter copies the result.
- **Web search** — `g rust` → Google, plus `yt` / `w` / `gh`; or just type a URL.
- **Windows Settings** — `bluetooth`, `display`, `wifi`, `startup apps`, … open the right page.
- **Commands** — `sleep`, `lock`, `shutdown`, `restart`, `kill <app>`, `em <emoji>` (out-of-process plugins).
- **Most-used** — an empty summon shows the apps and folders you use most.
- **Light / dark** — follows your Windows theme, live.

## Usage

Summon with **Ctrl+Space**. Change it any time — type `shortcut`, or right-click the tray
icon → **Change shortcut…**, then press your new combo. Type to search; ↑/↓ to select;
Enter to run; Esc to dismiss. Ordo lives in the tray — right-click for options and Quit.

**Searching files in other folders?** Type **`add folder`** and pick one (or `add folder
D:\Path` to add it directly). Ordo indexes it instantly and remembers it — no config editing.

## Privacy

Ordo has **no telemetry**. It touches the network only to (a) check for updates and
(b) open URLs you explicitly choose. Nothing about what you search or launch ever leaves
your machine.

## License

Ordo is free to use. © 2026 Aayush Sharat. All rights reserved. A formal freeware license
will accompany a future release.
