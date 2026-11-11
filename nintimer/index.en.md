---
layout: page
title: Nintimer
lang: en
---

[日本語](index.md)

**A presentation timer that lets you keep track of time without getting distracted by it.**

It sits small in a corner of the screen you're projecting, so you can check the time without looking away from the screen. It doesn't beep or flash when time is up, and it doesn't interfere with the keys you use to move between slides. If you enter start and end times, you don't even need to start it.

You can use it even where you can't use a presenter view (such as PowerPoint's Presenter View).

> **Nintimer is currently a free public beta.** If you notice anything, let us know through the [support contact](support.en.md). Known problems are listed in [Known issues](known_issues.en.md).

## What it does

- **Stays out of your way** — It's small and semi-transparent, and it doesn't beep or flash when time is up. It shows only the time, colors, and a thin bar, with no words like "Waiting."
- **No need to start it for a fixed time slot** — In Settings, enter start and end times, such as 13:00 to 13:30, and select **OK**. At 13:00, it starts timing on its own, even if you restart Nintimer or the date changes. The number shows the current time, and the thin bar shows how much time is left. Set it up the day before or during the break, and you won't forget to start it when your talk begins.
- **Leaves your slide keys alone** — It doesn't take the keyboard focus, so your keys for moving between slides still go to your presentation app. You can control the timer with just your mouse.
- **Works during a full-screen slide show** — Right-click the timer to start, pause, or open Settings. If it gets in the way, drag it somewhere else.
- **For talks that don't go as planned** — With a time limit or counting up, if something goes wrong, right-click and select **Pause**, and then **Resume** to continue from where you paused (the paused time isn't counted). If your presentation didn't actually start, select **Pause**, and then **Start over** to time again from zero. When you finish, select **Pause**, and the value at that moment stays on screen.
- **Three timing modes** — A time limit (for example, 20 minutes), start and end times (for example, 13:00 to 13:30), or counting up. When time is up, the timer turns red, and with a time limit it counts the overtime, like `+03:05`.
- **English and Japanese** — It follows the Windows display language, and you can also choose the language in Settings.

## Requirements

| | |
|---|---|
| OS | Tested on Windows 11 (64-bit, x64) |
| .NET | **Not required.** Everything it needs to run is included |
| Presentation app | Tested with full-screen slide shows in LibreOffice Impress, and in PowerPoint at 100% scale |
| Display scale | Tested at 100%, 150%, and 200% |

For details on the environments we've tested, see [Known issues](known_issues.en.md).

## Get Nintimer

### Microsoft Store version (recommended)

<https://apps.microsoft.com/detail/9N7LCWZ81GSC>

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
| 1.0.2 | `nintimer.exe` | `3F7E2B989F3152F4D3A04B69D8A599276F0DD6D770E19767D4CD9E17AC297C1B` |

If the value doesn't match, don't use the file.

## Getting started

1. Run `nintimer.exe` (start the Microsoft Store version from the Start menu).
2. A small timer appears in the upper-right corner of the screen, and an icon appears in the system tray.
3. Right-click the timer or the tray icon, select **Settings...**, set your time limit or times, and select **OK**.
4. When your presentation starts, double-click the timer, or right-click it and select **Start**. (If you set start and end times, the time window stays active once you select **OK**, even after you restart Nintimer, so you don't need to start it.)
5. To stop timing, right-click and select **Pause**. The value at that moment stays on screen. To continue, select **Resume**; to time again from zero, select **Start over** (with a time limit or counting up).

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
