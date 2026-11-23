---
layout: page
title: How to Collect Logs
lang: en
---

When HamonPlayer doesn't work as expected, follow these steps to get the records (the log) we need to look into it. Include them when you [contact support](support.en.md).

**The log includes the locations of your song files (folder names and song file names).** These locations may include your Windows user name (for example, `C:\Users\<user name>\Music\…`). **Always read the copied text yourself before you send it.** If there's anything you don't want to share, remove it or replace it with something like `***` before you send it.

## 1. Open the log

HamonPlayer writes a record of what it does to one file per month.

1. Right-click the HamonPlayer icon in the system tray, and select **History…**. The search window opens, showing History.
2. At the bottom of the window, select **Show actions**.
3. Select **Open log**, which appears at the bottom. This month's log opens. (If there's no log for this month, the log folder opens.)

If HamonPlayer doesn't start, or you can't open the log this way, type `%LOCALAPPDATA%\HamonPlayer\logs` in the address bar of File Explorer and open it. The files are named `hamon-<year><month>.log` (for November 2026, `hamon-202611.log`). You can open them in Notepad.

If you use the **Microsoft Store version** and there's no `HamonPlayer` folder in that location, Windows has redirected it. In File Explorer, type `%LOCALAPPDATA%\Packages` in the address bar and open it. Then open the folder whose name contains `HamonPlayer`, and look in `LocalCache\Local\HamonPlayer\logs`.

## 2. Copy the lines we need

The log has a whole month of records, so it gets long. **Copy only the lines from around the time the problem happened.**

1. Think of when the problem happened (as closely as you can).
2. Select the lines from a little before that time to a little after it, copy them, and paste them into your support request (or the body of your email).
3. **Read what you pasted.** If it includes anything you don't want to share, such as folder names, song names, or your user name, remove it or replace it with something like `***`.

### What the log looks like

Each line has a date and time, and what happened.

```
2026-11-14 07:21:47.098 INFO  Play: C:\Users\***\Music\Artist\Album\01 Song.mp3
2026-11-14 07:24:10.512 INFO  Sound from another app: chrome (pid 12345)
2026-11-14 07:24:10.513 INFO  Auto-pause
2026-11-14 07:26:58.407 INFO  End: Skip C:\Users\***\Music\Artist\Album\01 Song.mp3
```

It mainly records:

- When HamonPlayer started and exited, and its version
- The locations of the songs it played, and how each one ended (played to the end, skipped, or couldn't play)
- Actions such as Pause, the queue, and Like, and changes to the settings
- The names (process names) of apps that played sound when HamonPlayer auto-paused
- If you use phone sync, the model name of your phone and the number of songs synced
- How many songs it found in your music folders, and what went wrong (folders it couldn't read, saves that failed, and so on)

When you use HamonPlayer in English, the log is written in English too.

### If you can't find the lines

- Logs older than 12 months are deleted.
- If you can't find a record of what happened, **make the problem happen again** before you copy the log. Not finding a record can itself be a clue, so please tell us.

## 3. Please also tell us

The log alone often isn't enough, so please include the following. **With the first three, we can look into most problems.**

- **What you did and what happened.** If you can, list the steps in order, and tell us when it happened.
- **The HamonPlayer version.** Right-click the icon and open **Help**. The version is on the last line (for example, `HamonPlayer 1.0.6`). Also tell us whether it's the Microsoft Store version or the setup.exe version.
- **The Windows version.** "Edition", "Version", and "OS build" in Settings > System > About.
- If the icon is red, the message you see when you point at the icon.
- If a song doesn't play, the format of that song file (its extension, such as mp3 or m4a).
- If HamonPlayer pauses by itself, the name of the app that was playing sound at that time.

You usually **don't** need to send the settings file (`settings.json`) or the play data (`values.tsv`), because both contain the locations of your music folders. If we need them, we'll ask. **Don't send the song files themselves.**

## Where to send it

See [Support](support.en.md).

**Don't include logs you haven't read and checked, personal information, credentials, or details of vulnerabilities that haven't been made public in a public issue.**
