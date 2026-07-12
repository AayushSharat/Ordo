# Ordo

A fast, featherweight keyboard launcher for Windows. Press **Ctrl+Space**, type, and
instantly launch apps, find files, do quick math, search the web, open Windows Settings,
or run commands — all from one bar.

Built in native Rust (no Electron, no web runtime), so it stays tiny and instant:
~2–4 MB idle RAM, 0% idle CPU, a ~1.5 MB binary, and results in well under a frame.

### 🌐 Website & demo video → **[ordo-aayushsharat.vercel.app](https://ordo-aayushsharat.vercel.app)** · 📝 [Changelog](https://ordo-aayushsharat.vercel.app/changelog.html)

## Download

**[⬇ Download Ordo (installer)](https://github.com/AayushSharat/Ordo/releases/latest/download/OrdoSetup.exe)** — per-user, no admin needed. Recommended.

- **Portable:** [Ordo-portable.zip](https://github.com/AayushSharat/Ordo/releases/latest/download/Ordo-portable.zip) — unzip and run `ordo.exe`.
- Or browse [all releases & files](https://github.com/AayushSharat/Ordo/releases/latest) (each release also ships a `SHA256SUMS` to verify your download).

### ⚠️ Windows blocks or deletes the download? (It's a false alarm)

Ordo isn't **code-signed** yet, so Windows doesn't recognize the publisher and may treat
it as suspicious. Ordo is **open, has no telemetry**, and its source of updates is pinned
and SHA-256-verified — but Windows can't know that without a signature. Two things you
might see:

1. **SmartScreen** — *"Windows protected your PC."* Click **More info → Run anyway**.
2. **Defender removes the file** (*"Threat found"*, file deleted/quarantined). This is a
   **false positive**. To keep it:
   - Open **Windows Security → Virus & threat protection → Protection history**.
   - Find the Ordo item → **Actions → Allow / Restore**.
   - Or before downloading, add the Ordo install folder to **exclusions**
     (`%LOCALAPPDATA%\Programs\Ordo`).

Code signing (which removes both warnings for good) is on the roadmap.

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

## Feedback

Found a bug or have an idea? Please open an issue — it genuinely shapes what gets built next:

- 🐛 **[Report a bug](https://github.com/AayushSharat/Ordo/issues/new?template=bug_report.yml)**
- 💡 **[Request a feature / share feedback](https://github.com/AayushSharat/Ordo/issues/new?template=feature_request.yml)**
- Or browse [existing issues](https://github.com/AayushSharat/Ordo/issues).

## Changelog

See **[CHANGELOG.md](CHANGELOG.md)** (or the [web version](https://ordo-aayushsharat.vercel.app/changelog.html))
for what's new in each release. In-app, updates appear as an **"Update Ordo"** row when you
summon it — press Enter to install.

## Privacy

Ordo has **no telemetry**. It touches the network only to (a) check for updates and
(b) open URLs you explicitly choose. Nothing about what you search or launch ever leaves
your machine.

## License

Ordo is free to use. © 2026 Aayush Sharat. All rights reserved. A formal freeware license
will accompany a future release.
