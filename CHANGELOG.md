# Changelog

All notable changes to Ordo. Updates install themselves — summon Ordo and press
**Enter** on the "Update Ordo" row. Also on the web:
[ordo-aayushsharat.vercel.app/changelog.html](https://ordo-aayushsharat.vercel.app/changelog.html).

## [0.2.4] — 2026-07-17

- **Fixed:** **Newly installed apps show up without restarting Ordo.** Ordo now re-scans
  your installed apps each time you summon it (and periodically in the background), so an
  app you just installed appears within seconds instead of sometimes not showing up until
  you restarted Ordo.
- **Fixed:** **Updating no longer forgets your most-used apps and added folders.** After the
  earlier rename, updating across it could land you in fresh, empty data — so Ordo appeared
  to forget your history and the folders you'd added to search. Ordo now carries that data
  forward automatically on first launch (your old data is left in place as a backup).

## [0.2.3] — 2026-07-14

- **Fixed:** **The tray icon now reliably appears when Ordo starts with Windows.** If Ordo
  launched before the taskbar was ready at sign-in, its tray icon could go missing — so it
  looked like Ordo hadn't started, even though the hotkey still worked. Ordo now re-adds its
  icon as soon as the taskbar is ready, and again if Explorer restarts.

## [0.2.2] — 2026-07-12

- **Fixed:** **Updates now reach you automatically.** Ordo re-checks for new versions
  every few hours while it's running, so you no longer have to restart it (or reboot) to
  get an update. Previously it only checked once at startup, so a long-running instance
  could miss releases. (Existing users: this kicks in once you're on 0.2.2 — to get 0.2.2,
  right-click the tray icon → **Check for updates**, or quit and reopen Ordo.)

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

[0.2.4]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.4
[0.2.3]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.3
[0.2.2]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.2
[0.2.1]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.1
[0.2.0]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.0
[0.1.0]: https://github.com/AayushSharat/Ordo/releases/tag/v0.1.0
