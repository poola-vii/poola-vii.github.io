---
layout: page
title: How to Collect Logs
lang: en
---

When TwoTile doesn't work as expected, follow these steps to get the information we need to look into it. Include it when you [contact support](support.en.md).

This page is for TwoTile 1.0.9 and later. Earlier versions are shown only in Japanese.

**TwoTile doesn't write logs to a file.** It keeps its log only in the app, and the log is gone when you exit. **Copy it before you exit the app.**

**Always read the copied text yourself before you send it.** It includes window titles. If there's anything you don't want to share, remove it before you send it.

## 1. Copy the log while TwoTile is running

1. Right-click the TwoTile icon in the system tray, and select **Settings...**.
2. On the **General** tab, select **Open debug view**. You can close Settings with **Cancel**.
3. A window named "TwoTile - Debug view" opens. It shows up to 50 recent arrangements, warnings, and errors, newest first.
4. Select **Copy log** at the lower left. The log is copied to the clipboard.
   - To share only some lines, select those lines first and then copy them. To select more than one line, hold down Ctrl and select each line.
   - You can also use the keyboard: **Ctrl+A** selects all, and **Ctrl+C** copies.
5. Paste it into your support request.
6. **Read what you pasted.** Check that the window titles don't include anything you don't want to share, such as file names or page titles. If they do, remove it or replace it with something like `***`.

### What the copied text looks like

It starts with the TwoTile version and the Windows version, which we need to look into the problem.

```
TwoTile v1.0.9 debug view
Windows: Microsoft Windows NT 10.0.26200.0
Copied at: 2026-09-18 08:02:44

[2026-09-18 08:02:20] [Adjustment] [Adjust] "Window title" (ClassName) (980,496,600,400) -> (0,0,1280,1392)
[2026-09-18 08:02:16] [Adjustment] [Adjust] "Another window" (ClassName) (44,52,1129,635) -> (0,0,1280,1392)

* Before you paste this, check that it doesn't include anything you don't want to share, such as window titles.
```

An `[Adjust]` line means "TwoTile moved this window from this position to this position." The four numbers in parentheses are the left edge, top edge, width, and height.

### If nothing is logged

- When you restart TwoTile, the earlier log is gone. **Make the problem happen again** before you copy the log.
- If TwoTile hasn't arranged anything, the log is empty (the copied text shows "(No log entries to show)"). Then the fact that nothing happened is itself a clue. Copy and send it as it is.

## 2. If TwoTile doesn't start

If TwoTile fails to start, a window named **"TwoTile startup error"** appears.

1. While the window is shown, press **Ctrl+C**. All the text in the window is copied to the clipboard (this is standard Windows behavior).
2. Paste it into your support request.
3. Read what you pasted, and remove anything you don't want to share (file paths may include your user name).

If TwoTile exits without showing a window, please tell us that.

## 3. Please also tell us

The log alone often isn't enough, so please include the following. **With the first three, we can look into most problems.**

- **What you did and what happened.** If you can, list the steps in order.
- **The TwoTile version.** It's shown at the top of the system tray menu (for example, `TwoTile v1.0.9`). Also tell us whether it's the Store version or the portable version.
- **The Windows version.** "Edition", "Version", and "OS build" in Settings > System > About.
- Your display setup: the number of displays, and the resolution and scale of each one (Settings > System > Display).
- The name of the app, and which window doesn't work as expected.
- Your TwoTile settings: the grid settings, and whether you have exclusion rules.

You **don't** need to send `%APPDATA%\TwoTile\config.json`, because it contains window titles (in the exclusion rules). If we need it, we'll ask.

## Where to send it

See [Support](support.en.md).

**Don't include raw logs, personal information, credentials, or details of vulnerabilities that haven't been made public in a public issue.**
