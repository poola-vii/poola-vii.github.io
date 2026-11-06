---
layout: page
title: Nintimer
lang: en
---

[日本語](index.md)

**A presentation timer that shows the time left in a corner of the screen you're projecting.**

Even where you can't use a presenter view (such as PowerPoint's Presenter View), Nintimer puts a small, semi-transparent timer on top of your slides, on the same screen. You can see how much time is left without looking back and forth between your laptop and the screen.

> **Nintimer is currently a free public beta.** If you notice anything, let us know through the [support contact](support.en.md). Known problems are listed in [Known issues](known_issues.en.md).

## What it does

- **Three timing modes** — A time limit (for example, 20 minutes), start and end times (for example, 13:00 to 13:30), or counting up.
- **Colors and a progress bar** — Gray while waiting or stopped, white while timing, and red when time is up, with the overtime shown as `+03:05`. A bar shows how much time is left.
- **Stays out of your way** — It doesn't take the keyboard focus, so your keys for moving between slides still go to your presentation app. It doesn't make sounds.
- **Works during a full-screen slide show** — Right-click the timer to start, stop, or open Settings. Drag it to move it.
- **Start over anytime** — If your presentation didn't actually start, right-click, select **Stop**, and then **Start over** to time again from zero.
- **English and Japanese** — It follows the Windows display language, and you can also choose the language in Settings.

## Requirements

| | |
|---|---|
| OS | Tested on Windows 11 (64-bit, x64). ARM and 32-bit Windows aren't supported |
| .NET | **Not required.** Everything it needs to run is included |
| Presentation app | Tested with full-screen slide shows in LibreOffice Impress |
| Display scale | Tested at 100%, 150%, and 200% |

For other environments, see the table in [Known issues](known_issues.en.md).

## Get Nintimer

### Microsoft Store version (recommended)

<!-- TODO: Add the link after Nintimer is submitted to the Store -->

Search for "Nintimer" in the Microsoft Store and install it. The Store keeps it up to date. **On PCs with Smart App Control turned on, use the Microsoft Store version.**

### Portable version

**For PCs that can't use the Microsoft Store.** No installation is needed. Put `nintimer.exe` anywhere you like and run it.

- Download: <https://github.com/poola-vii/Nintimer-releases/releases>
- When you recommend Nintimer to others, share this page instead of the file. If someone gives you the file, check that it's genuine with "Check the file you downloaded" below before you use it (the rules for sharing are in §4 of the [Terms of Use](terms.en.md)).

**The portable version isn't signed.** Because of this:

- **The first time you start it, Windows shows "Windows protected your PC."** Select **More info**, and then select **Run anyway**.
- On PCs with Smart App Control turned on, it can't start. Use the Microsoft Store version instead.

#### Check the file you downloaded

After you download it, check that it's the same as the one on the distribution site. Run the following in PowerShell, and check that the value matches the table below.

```pwsh
Get-FileHash .\nintimer.exe -Algorithm SHA256
```

| Version | File | SHA-256 |
|:---|:---|:---|
| 1.0.1 | `nintimer.exe` | `4398E5AFA19ACA2D06961CF7A78F9833EC9699482F5E04D377375D8B3A1712F3` |

If the value doesn't match, don't use the file.

## Getting started

1. Run `nintimer.exe` (start the Microsoft Store version from the Start menu).
2. A small timer appears in the upper-right corner of the screen, and an icon appears in the system tray.
3. Right-click the timer or the tray icon, select **Settings...**, set your time limit or times, and select **OK**.
4. When your presentation starts, double-click the timer, or right-click it and select **Start**. (If you set start and end times, the time window starts when you select **OK**, so you don't need to start it.)
5. When you finish, right-click and select **Stop**. The value at that moment stays on screen.

### Language

Nintimer appears in Japanese when the Windows display language is Japanese, and in English otherwise. You can also choose the language with **言語 / Language** at the bottom of Settings. Changing the language and selecting **OK** restarts the timer, so choose it before your presentation.

**On Japanese Windows, right-click the timer or the system tray icon, select 設定..., set 言語 / Language to English, and then select OK.** Until then, the menu is in Japanese. 設定... is the only item that ends with three dots.

**Nintimer doesn't start automatically.** Start it when you give a presentation.

Your settings are saved in `%APPDATA%\nintimer\config.json`. To stop using the portable version, delete `nintimer.exe` and this folder.

## If something goes wrong

- [Known issues](known_issues.en.md) — Known problems and tested environments
- [Support](support.en.md) — How to report problems and collect the log

## More

- [Changelog](CHANGELOG.en.md)
- [Terms of Use](terms.en.md) (reference translation; the Japanese version is the official one)
- [Privacy Policy](privacy_policy.en.md) (reference translation) — **Nintimer doesn't connect to the internet.**
- [Third-Party Notices](third_party_notices.en.md)

You can also read the Terms of Use, the Third-Party Notices, and the official download sources in the app. Right-click the system tray icon and select **Terms, licenses, and download sources**.

---

© 2026 poola-vii
