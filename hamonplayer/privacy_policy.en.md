---
layout: page
title: Privacy Policy
lang: en
---

**Established: 2026-11-22 / Applies to: HamonPlayer 1.0.1 (Windows version; Microsoft Store version and setup.exe version)**

> **This is a reference translation.** The [Japanese version](privacy_policy.md) of this Privacy Policy is the official one. If this translation and the Japanese version differ, the Japanese version prevails (§10).

> **This document hasn't been reviewed by a professional.**
>
> This page explains what the **app** handles. For **what GitHub records when you view this site** (visitors' IP addresses), see [Privacy on this site](/privacy.html) (in Japanese).

`poola-vii` (an individual living in Japan; "we" or "us"), who provides HamonPlayer (the "Software"), handles information as follows when you use the Software.

## Summary

- **The Software doesn't connect to the internet.**
- **We don't collect your information.**
- **All files the Software creates stay on your PC (and in places you choose).**
- **The Software uses the network only when you turn on "Allow syncing to your phone."** Even then, it talks only to the phones you connect, inside your home network. It doesn't use any outside server.

## 1. Information we don't collect

The Software doesn't do any of the following:

- Send usage data, operation history, or activity logs (telemetry or analytics)
- Get or send information that identifies you or your PC (except that, when you turn on phone sync, your PC answers with its name inside your home network, as described in §5)
- Show ads or collect information for ads
- Connect to any server on the internet, including to check for updates or to get song information (such as song names or album art)

**How to use** and **What's new** under **Help** in the app open pages that are included in the app, in your browser. They don't open pages on the internet.

## 2. Information handled on your PC

To work, the Software handles the following information **only on your PC**. **It doesn't send it anywhere** (except for phone sync in §5). For other apps, it handles only whether they're playing sound, and their process names and ID numbers. It doesn't read other apps' screens or text, or what you type on the keyboard.

| Information | Purpose | Where it's kept |
|:---|:---|:---|
| The locations (full paths), sizes, and dates of the files in your music folders | To find and play songs | The play data and record files in §3 below |
| Song tags (artist, title, album, and so on) and album art | To show song names and to search | Tags: the record files in §3 below. Album art: in memory only |
| Measured loudness of each song | To play all songs at a similar volume | The record files in §3 below |
| Play data (for each song, how long until it comes back, and its order) | To choose the next song | The play data and backups in §3 below |
| History of songs played and actions | To show History | The history files in §3 below. Deleted after 12 months |
| The song and position when you exit | To continue where you stopped the next time it starts | The record files in §3 below |
| Your settings (music folders, volume, play schedule, keyboard shortcuts, apps to ignore, and so on) | To restore them the next time you start the app | The settings file in §3 below |
| Whether other apps are playing sound (process names and ID numbers) | To pause when another app plays sound | In memory only. The name of the app that caused a pause is also written to the log |
| The current song's name, artist, album, and album art | To show them in the Windows media controls (such as in quick settings) | Given to Windows (on your PC). The Software doesn't save them |
| A record of what the app does (the log) | To investigate problems | The log files in §3 below. Deleted after 12 months |
| Information for phone sync (the PC's certificate, the model names of connected phones, hashes of their pairing tokens, and when each phone was connected and last synced) | To recognize and connect phones | The files in §3 below. Created only if you use phone sync |

## 3. Files the Software creates

| | |
|---|---|
| Location | `%LOCALAPPDATA%\HamonPlayer\` (usually `C:\Users\<user name>\AppData\Local\HamonPlayer\`) |
| Settings file | `settings.json`. A text (JSON) file you can open in Notepad |
| Play data | `values.tsv`. One line per song, with the location of the song file and two numbers |
| Backups | `backups\`. Copies of the play data, made each time the app starts and before the first save of each day. The 30 newest are kept, and for older ones, one per day for 30 days and one per month for 12 months. You can choose where they go with **Backup folder** in Settings. For the Microsoft Store version, they go to `HamonPlayer\backups` in your Documents folder by default (so that uninstalling doesn't delete them). If you sync your Documents folder with OneDrive or a similar service, the backups are synced too (the sync app sends them, not the Software) |
| Record files | `tags.tsv` (tags), `loudness.tsv` (loudness), `resume.tsv` (the song and position when you exit) |
| History | `history\history-<year><month>.tsv`. One file per month. Files older than 12 months are deleted |
| Log files | `logs\hamon-<year><month>.log`. One file per month. Files older than 12 months are deleted when the app starts. They contain the locations of song files, actions, the names of apps that played sound when the app auto-paused, the model names of connected phones, and so on |
| Quarantine folder | `quarantine\`. Keeps lines of play data that couldn't be read, settings files that couldn't be read, and data that wasn't saved because it looked wrong. It isn't deleted automatically |
| Phone sync | `carry-out-cert.pfx` (the PC's certificate) and `carry-out-phones.json` (connected phones). Created when you allow syncing to your phone |

When you use **Export play data…** in Settings, the Software writes one copy of your play data to the place you choose.

If you use the Microsoft Store version and there's no `HamonPlayer` folder in the location above, Windows has redirected it to an app-specific location (under `%LOCALAPPDATA%\Packages\`) (if you used the setup.exe version first and the folder is in the location above, the Store version uses it too).

### Registry

- The installer of the setup.exe version registers HamonPlayer so that it appears in **Installed apps** in Windows. This is removed when you uninstall.
- Only when you turn on **Start HamonPlayer when Windows starts** in Settings, the Software registers itself to start with Windows (for the setup.exe version, a value in the registry key `HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run`; for the Store version, a Windows startup task). Turning it off removes the registration. For the setup.exe version, uninstalling also removes it.

### How to remove everything

To stop using the Software:

- **setup.exe version**: Uninstall it from Windows Settings. The installed files and the registration to start with Windows are removed. **Your play data and settings are kept, and their location is shown.** If you don't need them, delete the `%LOCALAPPDATA%\HamonPlayer` folder yourself.
- **Microsoft Store version**: Uninstall it from Windows Settings. The files in the app-specific location (play data, settings, and so on) are deleted too. The backups in `HamonPlayer\backups` in your Documents folder are kept. If you don't need them, delete them yourself. If the `%LOCALAPPDATA%\HamonPlayer` folder is still there (when you used the setup.exe version first), delete it yourself too.
- For both versions, if you changed the backup folder, the backups in that folder are kept. If you don't need them, delete them yourself. The same goes for play data files you exported.

## 4. Third-party software

See the Third-Party Notices for the software included in the Software. None of it connects to the internet.

## 5. Phone sync (communication inside your home network)

The Software can send your top songs to a phone on the same home network. The phone version (Android) will be released later. When it is, we'll add the information the phone version handles to this policy.

- **It's off by default.** It works only when you turn on **Allow syncing to your phone** on the **Phone sync** tab in **Settings…**.
- While it's on, your PC listens inside your home network on TCP and UDP port 47823 (or another free TCP port if that one is in use). It accepts connections only from addresses inside a home network (the private addresses 10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16, the link-local addresses 169.254.0.0/16 that don't pass through a router, and the addresses of the PC itself, 127.0.0.0/8), and closes all others. However, if you connect your PC to an outside network, such as at a café, and that network uses addresses in the same ranges, your PC listens there too (see the Windows Firewall item below).
- When a phone sends a signal to look for PCs, your PC answers with its name (the Windows computer name), its port, its certificate fingerprint, and whether it's accepting new phones. It answers only signals from addresses in the same ranges. Other devices on the same network can also learn your PC's name by sending this signal. The certificate fingerprint stays the same for a long time on each PC, so they can also tell from the answer that it's the same PC.
- To connect a new phone, you type the 6-digit code shown on your PC into the phone. The code is accepted only while that tab is open in the Settings window (even if the window is behind other windows), and it changes every 5 minutes.
- The communication is encrypted (TLS) with a certificate created on your PC.
- **What the PC sends to the phone**: the song files chosen for sync, the play data lines for those songs (including where the song files are on your PC), song names and albums, volume adjustment values, and the PC's name.
- **What the PC receives from the phone**: the phone's model name, and records of what you played on the phone (songs played, Skip, Like, and so on). When **Add what you played on the phone to this PC** is on in Settings, these are added to the play data on your PC.
- None of this goes through any server on the internet, and none of it reaches us.
- The first time you allow syncing, Windows Firewall asks for permission.
- Your PC remembers the networks where your phone has synced as home networks, and it doesn't listen when it is connected to other networks, such as at a café. It remembers only the ID that Windows gives each network (kept in the settings file), and it doesn't send it outside your PC. Until you connect a phone, and while the **Phone sync** tab in Settings is open, your PC listens on any network.
- If you select **Remove** for a phone under **Connected phones**, that phone isn't accepted from its next connection on.

## 6. Information on download sites and the support contact

We use **GitHub** and the **Microsoft Store** to distribute the Software, and **GitHub** and email for support. **Your use of these services is subject to the policies of their operators**, not ours.

- Anything posted to the support contact on GitHub (https://github.com/poola-vii/support) **can be read by anyone** on GitHub. Before you post, check that it doesn't include information you don't want to share. The log includes the locations of your music folders, which may include your Windows user name.
- **We don't make public** what you send us by email or your email address. When we share what we found with other users, we make sure you can't be identified.
- We use what you send us and your email address only to investigate and respond to it. We don't use them for any other purpose, and we don't give them to third parties.

## 7. Children

The Software isn't aimed at any particular age group. As described above, it doesn't collect any information about you.

## 8. Changes to this policy

We'll update this policy when the Software's behavior changes. We'll announce changes on the distribution site (https://github.com/poola-vii/HamonPlayer-releases) and the official site (https://poola-vii.github.io/hamonplayer/).

## 9. Contact

https://github.com/poola-vii/support (recommended), or email `poola.vii.support@gmail.com`. For details, see "Support."

The Software is provided by an individual living in Japan. Under Microsoft's rules, the provider's real name is shown on the Microsoft Store listing page.

## 10. Language

The Japanese version of this policy is the official one. This English reference translation is provided to help you understand it. If this translation and the Japanese version differ, the Japanese version prevails.
