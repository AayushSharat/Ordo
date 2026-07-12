# Changelog

All notable changes to Ordo. Updates install themselves — summon Ordo and press
**Enter** on the "Update Ordo" row. Also on the web:
[ordo-aayushsharat.vercel.app/changelog.html](https://ordo-aayushsharat.vercel.app/changelog.html).

## [0.2.1] — 2026-07-12

- **Fixed:** You can now **edit anywhere in the search bar**. Move the cursor with
  **←/→** (hold **Ctrl** to jump by word; **Home/End** to jump to the ends) and fix a
  typo mid-query without deleting everything after it. **Backspace** and **Delete** act
  at the cursor.
- **Added:** **Cube root** in the calculator — `cbrt(27)` → 3, alongside `sqrt`.

## [0.2.0] — 2026-07-11

- **Added:** **Add any folder to search.** File search previously covered only your main
  folders (Desktop, Documents, Downloads, Pictures, Videos, Music). Now type
  **`add folder`** to pick any folder — or **`add folder D:\Path`** to add it directly.
  Ordo indexes it instantly and remembers it, with no config editing.

## [0.1.0] — 2026-07-11

- First public release. A fast, featherweight keyboard launcher for Windows:
  - App launch (Start Menu + Store apps), instant Everything-style file search,
    inline calculator, web search (`g`, `yt`, `w`, `gh`, or a URL), Windows Settings
    pages, and out-of-process commands (`sleep`, `lock`, `shutdown`, `restart`,
    `kill <app>`, `em <emoji>`).
  - Most-used view on an empty summon, live light/dark theming, a rebindable hotkey,
    and consent-based, SHA-256-verified auto-update.
  - Native Rust — ~3 MB idle RAM, 0% idle CPU, a ~1.5 MB binary, no telemetry.

[0.2.1]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.1
[0.2.0]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.0
[0.1.0]: https://github.com/AayushSharat/Ordo/releases/tag/v0.1.0
