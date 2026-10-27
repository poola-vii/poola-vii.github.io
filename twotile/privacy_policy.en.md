---
layout: page
title: Privacy Policy
lang: en
---

**Established: 2026-09-18 / Revised: 2026-09-20 (product renamed to TwoTile), 2026-09-26 (added the documents bundled in Help), 2026-10-06 (settings backups limited to the 10 newest), 2026-10-12 (added Vector and the email contact), 2026-10-26 (added this English reference translation) / Applies to: TwoTile 1.0.9 (Microsoft Store version and portable version)**

> **This is a reference translation.** The [Japanese version](privacy_policy.md) of this Privacy Policy is the official one. If this translation and the Japanese version differ, the Japanese version prevails (§9).

> **This document hasn't been reviewed by a professional.**
>
> This page explains what the **app** handles. For **what GitHub records when you view this site** (visitors' IP addresses), see [Privacy on this site](/privacy.html) (in Japanese).

`poola-vii` (an individual living in Japan; "we" or "us"), who provides TwoTile (the "Software"), handles information related to your use of the Software as follows.

## Summary

- **The Software doesn't communicate over the internet.**
- **We don't collect information about you.**
- **All files the Software creates stay on your PC.**

## 1. Information we don't collect

The Software doesn't do any of the following:

- Send usage, activity history, or operation records (telemetry or analytics)
- Get or send information that identifies you or your PC
- Show ads, or get information for ads
- Connect to any server, including to check for updates

The Software has no feature for communicating with anything outside your PC.

## 2. Information handled on your PC

To work, the Software handles the following information **only on your PC**. **It doesn't send it anywhere.**

| Information | Why | Where it's kept |
|:---|:---|:---|
| Titles, class names, positions, and sizes of open windows | To choose which windows to arrange and where to place them | In memory only. Gone when you exit |
| Recent arrangements, warnings, and errors (up to 1,000 entries) | To show them in the debug view | In memory only. Gone when you exit. **Never written to a file** |
| Settings you choose (grid divisions, margins, exclusion rules, fixed-width rules, and so on) | To keep them the next time you start | The settings file in §3 below |

**Exclusion rules and fixed-width rules include the window titles you enter.** The settings file is on your PC, and we can't read it.

## 3. Settings file

| | |
|---|---|
| Location | `%APPDATA%\TwoTile\config.json` (usually `C:\Users\<user name>\AppData\Roaming\TwoTile\config.json`) |
| Format | Text (JSON). You can read it in Notepad or a similar app |
| Backups | Each time you change and save settings, TwoTile creates `config.json.<date and time>.bak` in the same place. **Only the 10 newest are kept; older ones are deleted automatically when settings are saved.** If the settings file is damaged and can't be read, its contents are kept in `config.json.<date and time>.invalid.bak`. Those aren't deleted automatically |

On a PC with no settings file in the location above, Windows may redirect the Microsoft Store version's settings to a location just for the app (under `%LOCALAPPDATA%\Packages\`). In that case, the settings are removed when you uninstall the Store version.

### How to remove it

When you stop using the Software:

- **Store version**: Uninstall it from Windows Settings. If there's a settings file in `%APPDATA%\TwoTile` above, **it stays after you uninstall**. Delete it yourself.
- **Portable version**: Delete `TwoTile.exe`. The settings file stays, so delete it yourself.
- For either version, deleting the whole `%APPDATA%\TwoTile` folder removes all settings and backups.

## 4. Third-party software

The Software uses **Microsoft Edge WebView2** to show Help. It shows only the documents bundled with the Software (the user manual, the Terms of Use, the Third-Party Notices, and the official download sources), and **never opens web pages**. Links in the documents don't open when selected; URLs are shown as text.

WebView2 creates data it needs to work in `%LOCALAPPDATA%\TwoTile\WebView2`. How WebView2 itself handles information is governed by Microsoft's terms.

For other software we use, see the [Third-Party Notices](third_party_notices.en.md).

## 5. Information at download sources and support contacts

We use **GitHub**, the **Microsoft Store**, and **Vector** to distribute the Software, and **GitHub** and email for support. **When you use these services, the policies set by each operator apply**, not ours.

- What you post on GitHub through the [support contact](support.en.md) becomes **readable by anyone** on GitHub. Before you post, check that it doesn't include anything you don't want to share.
- **We don't make public** what you send us by email or your email address. When we share what we found with other users, we make sure you can't be identified.
- We use what you send us and your email address only to look into what you reported and to reply. We don't use them for anything else, and we don't give them to third parties.

## 6. Children

The Software isn't intended for any particular age group. As described above, we don't collect any information about you.

## 7. Changes to this policy

When the way the Software works changes, we update this policy. When we do, we announce it at the [download source](https://github.com/poola-vii/TwoTile-releases) and on the official site.

## 8. Contact

<https://github.com/poola-vii/support> (recommended) or email `poola.vii.support@gmail.com`. For details, see [Support](support.en.md).

The provider of the Software is an individual living in Japan. The Microsoft Store listing shows the provider's real name, as Microsoft requires.

## 9. Language

The Japanese version of this Privacy Policy is the official one. This English reference translation is provided to help you understand it. If the Japanese version and this translation differ, the Japanese version prevails.
