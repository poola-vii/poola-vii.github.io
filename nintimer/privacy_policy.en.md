---
layout: page
title: Privacy Policy
lang: en
---

**Established: 2026-10-29 / Applies to: Nintimer 1.0.2 (Microsoft Store version and portable version)**

> **This is a reference translation.** The [Japanese version](privacy_policy.md) of this Privacy Policy is the official one. If this translation and the Japanese version differ, the Japanese version prevails (§9).

> **This document hasn't been reviewed by a professional.**
>
> This page explains what the **app** handles. For **what GitHub records when you view this site** (visitors' IP addresses), see [Privacy on this site](/privacy.html) (in Japanese).

`poola-vii` (an individual living in Japan; "we" or "us"), who provides Nintimer (the "Software"), handles information as follows when you use the Software.

## Summary

- **The Software doesn't connect to the internet.**
- **We don't collect your information.**
- **All files the Software creates stay on your PC.**

## 1. Information we don't collect

The Software doesn't do any of the following:

- Send usage data, operation history, or activity logs (telemetry or analytics)
- Get or send information that identifies you or your PC
- Show ads or collect information for ads
- Connect to any server, including to check for updates

The Software has no feature that communicates over the network. The "Terms, licenses, and download sources" window in the app doesn't open web pages either.

## 2. Information handled on your PC

To work, the Software handles the following information **only on your PC**. **It doesn't send it anywhere.** It doesn't read the content of your presentation (slides, or the screens or text of other apps). For other apps' windows, it handles only the window and process ID numbers and their state, such as whether they're visible or minimized.

| Information | Purpose | Where it's kept |
|:---|:---|:---|
| The timer's state (values while timing or stopped) | To show the timer | In memory only. It's gone when the app closes |
| Your settings (timer mode, time limit, start and end times, display size, progress bar position and direction, display language, timer position) | To restore them the next time you start the app | The settings file in §3 below |
| A record of when the timer's position was corrected automatically (the position before and after, and the positions and sizes of the displays at that time) | To investigate problems | The log file in §3 below |
| The ID numbers of the apps' windows you used most recently (window and process numbers, up to 8) | To give keyboard input back to your slide show or other app after you use the timer's menu, Settings, or other windows | In memory only. It's gone when the app closes |
| A record of when keyboard input was given back (the ID number of the window it was given back to, the ID number of the window that has keyboard input afterward, and whether it succeeded) | To investigate problems | The log file in §3 below |

## 3. Settings file and log file

| | |
|---|---|
| Location | `%APPDATA%\nintimer\` (usually `C:\Users\<user name>\AppData\Roaming\nintimer\`) |
| Settings file | `config.json`. A text (JSON) file you can open in Notepad |
| Log file | `nintimer.log`. Written only when the display setup changes and the timer's position is corrected automatically because it would otherwise be off screen, when keyboard input is given back to another window after you use the timer's menu, Settings, or other windows (including when that fails), when it can't set up the notifications about foreground window changes that it uses to give keyboard input back (at startup), and when the tray icon can't be shown. It doesn't include window titles or contents. When it grows beyond 256 KB, it's deleted and started again |

On a PC that doesn't have the `nintimer` folder in the location above, Windows redirects the Microsoft Store version to an app-specific location (under `%LOCALAPPDATA%\Packages\`). In that case, uninstalling the Store version also removes its settings and log.

### How to remove everything

To stop using the Software:

- **Microsoft Store version**: Uninstall it from Windows Settings. If `%APPDATA%\nintimer` exists, **it stays after you uninstall**. Delete it yourself.
- **Portable version**: Delete `nintimer.exe` and the `%APPDATA%\nintimer` folder.
- The Software doesn't write to the registry.

## 4. Third-party software

See the Third-Party Notices for the software included in the Software. None of it communicates over the network.

## 5. Information on download sites and the support contact

We use **GitHub** and the **Microsoft Store** to distribute the Software, and **GitHub** for support. **Your use of these services is subject to the policies of their operators**, not ours.

- Anything posted to the support contact (https://github.com/poola-vii/support) **can be read by anyone** on GitHub. Before you post, check that it doesn't include information you don't want to share.
- We use what you send us only to investigate and respond to it. We don't use it for any other purpose.

## 6. Children

The Software isn't aimed at any particular age group. As described above, it doesn't collect any information about you.

## 7. Changes to this policy

We'll update this policy when the Software's behavior changes. We'll announce changes on the distribution site (https://github.com/poola-vii/Nintimer-releases) and the official site (https://poola-vii.github.io/nintimer/).

## 8. Contact

https://github.com/poola-vii/support. For details, see "Support."

The Software is provided by an individual living in Japan. Under Microsoft's rules, the provider's real name is shown on the Microsoft Store listing page.

## 9. Language

The Japanese version of this policy is the official one. This English reference translation is provided to help you understand it. If this translation and the Japanese version differ, the Japanese version prevails.
