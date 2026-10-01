# Valkyrie

**A private memory for Claude.** Valkyrie runs on your Windows PC and gives Claude
(Desktop, Code, claude.ai and the phone app) a memory: a vault of plain Markdown
notes you own, a calendar, and a 3D view of everything you know.

## Install

1. Download **`Valkyrie-Setup.exe`** from the [latest release](https://github.com/System-Valkyrie/valkyrie/releases/latest).
2. Double-click it. If Windows shows "Windows protected your PC", click **More info**, then **Run anyway**
   (the app isn't code-signed yet).
3. Press **Install**. No admin rights, Python or anything else needed.

Windows 10 or 11 (64-bit), about 250 MB of disk.

## Updates

Valkyrie checks this page every few hours. When there's a new version, the
**Connect Claude** page shows **Update now**. One click downloads it, checks its
SHA-256 against the one published here, and updates in place. Your notes are never touched.

## Your data

Notes live in `Documents\Valkyrie Vault` as ordinary files. Uninstalling never deletes them.
Nothing is sent anywhere unless you turn on phone & web access (via your own free ngrok account).

See [CHANGELOG.md](CHANGELOG.md) for what changed in each version.
