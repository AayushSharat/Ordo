# Changelog

All notable changes to Ordo. Updates install themselves — summon Ordo and press
**Enter** on the "Update Ordo" row. Also on the web:
[ordo-aayushsharat.vercel.app/changelog.html](https://ordo-aayushsharat.vercel.app/changelog.html).

## [0.2.8] — 2026-08-06

- **New:** **Keep the screen awake while Ordo runs.** Type `screen awake` and Ordo offers one
  inverse action: turn it on when it is off, or turn it off when it is on. It uses a temporary
  Windows execution-state request and does not change your power-plan settings.
- **New:** **Create and edit `.env` files quickly.** Type `create .env` to choose a folder and
  create an empty file, or use `open .env` / `edit .env` to open an existing file in Notepad and
  save it normally.
- **Improved:** **Typing stays within the keystroke performance budget.** Preference matching
  reuses the query's lowercase key, and input echo is coalesced so normal fast searches avoid
  redundant full-scene paints.

## [0.2.7] — 2026-08-05

- **Fixed:** **Up and Down now recall your recent searches.** Ordo keeps session-local search
  history and restores your draft when you move past the newest entry.
- **Fixed:** **Mouse interaction and clipboard shortcuts now work.** Hover and click result rows,
  copy the query with **Ctrl+C**, and paste text with **Ctrl+V**.
- **Fixed:** **Installed app discovery is more complete.** Start Menu shortcuts now fill gaps when
  Windows' app list omits a classic app, and those shortcuts launch directly.
- **Improved:** **Rapid summon/hide cycles are faster.** Ordo keeps its render surface warm briefly
  after hiding, then releases it once genuinely idle. The release benchmark measured an 8.59 ms
  hotkey p95 while keeping hidden working set below the 15 MB budget.

## [0.2.6] — 2026-07-22

- **New:** **Pin your favorite apps, folders, and files.** Highlight any result and press
  **Ctrl+P** to pin it (press again to unpin), or type `pin <name>` / `unpin <name>`. Pinned
  items stay at the top when you summon Ordo, above your most-used list, and never fade out.
- **New:** **Reset your most-used history.** Type `reset recents` (or `clear history`) and press
  Enter to clear the most-used list. Your pinned items are kept.
- **Fixed:** **Installing an update no longer needs you to quit Ordo first.** An available update
  now applies on its own — Ordo closes itself gracefully, the update installs, and Ordo relaunches,
  with no manual Quit from the tray.
- **Improved:** **Lower CPU while the search bar is open.** Ordo no longer repeats text-layout work
  on every repaint, so an open Ordo sits at ~0% CPU.

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

[0.2.7]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.7
[0.2.8]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.8
[0.2.4]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.4
[0.2.3]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.3
[0.2.2]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.2
[0.2.1]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.1
[0.2.0]: https://github.com/AayushSharat/Ordo/releases/tag/v0.2.0
[0.1.0]: https://github.com/AayushSharat/Ordo/releases/tag/v0.1.0
