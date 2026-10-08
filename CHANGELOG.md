# Changelog

## v1.2.0 (2026-10-08)

**Valkyrie Health (new)**
- Valkyrie now watches itself and the PC it runs on, the same way the original Valkyrie Core does.
- **Uptime:** 7-day uptime for each part of Valkyrie, counted only while Valkyrie is running, so a sleeping PC isn't counted as an outage.
- **Self-repair:** a part that keeps using too much memory gets restarted automatically, at most once an hour.
- **PC checks:** drive health, a warning before your disk fills up, a pending Windows-update restart, unexpected shutdowns, and a reminder when your connector address is due for a change.
- **Nightly self-test:** if something's wrong, you get a Windows notification (at most once every 12 hours per problem).
- **Health card** on the Connect Claude page, with a **Run self-test** button and a status page that still loads if Valkyrie Mind is down.
- **A daily "Valkyrie Health" note** in your vault (Claude Knowledge → Reference), so Claude can see how Valkyrie is doing and tell you when something needs fixing.

**Mentor messages (suggested by a tester)**
- When your mentor leaves you a message, you get a notification, and the Connect page shows "1 new message" on the Mentor card. The daily Health note mentions it too, so Claude knows to check.

**Fixes**
- No more black command windows flashing up. Every background task Valkyrie runs (health checks, Claude connections, phone & web access, setup, uninstall) now stays invisible.

**Sync status (new)**
- A **Sync** pill in Valkyrie Mind shows whether Claude is talking to your memory: green when synced, amber when it's been quiet for a couple of days. Click it to see each Claude app (Claude Code, Claude Desktop, claude.ai / phone) and when it last used or saved a memory.
- **Claude Code status line:** connecting Claude Code now adds a small "✦ Valkyrie synced · Claude Code 2m ago" to its status bar. If you already have a status line of your own, it's left alone.


**Server-only mode (suggested by a tester)**
- Run Valkyrie as just the memory server for Claude, with no window, no tray icon and no Mind app. It uses less memory and wakes up less often while it waits.
- Turn it on with `Valkyrie.exe headless on` and off with `Valkyrie.exe headless off`. The setting is saved, so it stays that way after a restart.
- `Valkyrie.exe mentor on|off` and `Valkyrie.exe status` work from the command line too. Start-up and errors go to the log folder, and the self-test knows the Mind app is meant to be off.

**Calendar**
- The calendar health tools no longer report "Never synced with Google" as a problem. This edition keeps your calendar on your PC, and Claude now says that plainly.

## v1.1.0 (2026-10-01)

**Works on more PCs**
- PCs without the WebView2 component (and Windows Sandbox) no longer get a blank white or black window. Setup and Valkyrie Mind open in an Edge or Chrome window instead, automatically.
- Setup now has a normal Windows title bar, and its close button can't interrupt an install halfway through.

**Automatic updates**
- Valkyrie now checks for new versions. When one is out, the Connect Claude page shows **Update now**: one click downloads it, verifies it, and updates in place. Your notes are never touched.
- (Coming from 1.0.0? Install this version by hand once. Updates after this are one click.)

**Mentor link (new)**
- Let someone you trust connect their Claude to help yours: teach it rules, answer its questions, and troubleshoot. They only see the `Mentor` folder and Valkyrie's own logs, never your other notes. Everything they do is listed in `Mentor/Activity.md`, and you can turn it off any time. Find it on the Connect Claude page.

**Hearth Mode**
- Rewritten for everyone: you choose exactly which notes guests can see. Everything else, new notes included, stays hidden.
