---
layout: page
title: Known Issues
lang: en
---

Known limitations of TwoTile 1.0.9 (public beta), and the environments it has been tested in.

TwoTile is shown in English from version 1.0.9. Earlier versions are shown only in Japanese.

If you notice anything, let us know through the [support contact](support.en.md). We add what we learn to this page.

## By design

This is intended behavior that we don't plan to change.

### Only windows on the main display are arranged

TwoTile doesn't touch windows on other displays. They stay where you put them.

TwoTile sizes the grid from the work area of the main display, so arranging windows on other displays would pull them over to the main display. This behavior avoids that. When you move a window to another display, TwoTile stops managing it after a few seconds. Move it back to the main display to have it arranged again.

### Some windows aren't arranged

These windows are always left out:

- Maximized and minimized windows
- Windows that can't be resized (most dialog boxes, settings windows, and so on)
- Windows without a title, and child windows of other windows
- Tool windows (small helper windows that don't appear on the taskbar)

If a window is arranged when you don't want it to be, leave it out on the **Exclusion rules** tab of **Settings...** in the system tray menu.

### Windows beyond the number of cells aren't arranged

TwoTile arranges as many windows as there are cells, starting with the one in front. The rest stay where they are.

### Virtual desktops aren't distinguished

TwoTile doesn't look at which virtual desktop a window is on.

### The language follows the Windows display language

TwoTile is shown in Japanese when the Windows display language is Japanese, and in English otherwise. There's no setting to change it. If your Windows display language is English, TwoTile can't be shown in Japanese.

### TwoTile doesn't connect to the internet or tell you about updates

The app doesn't connect to the internet. When a new version comes out, the app doesn't tell you. The Microsoft Store updates the Store version. For the portable version, check the [download source](https://github.com/poola-vii/TwoTile-releases/releases).

## Things to keep in mind

### Windows take a moment to be arranged

TwoTile checks your windows every second and arranges them. So after you open or close a window, it takes 1 to 2 seconds for the windows to be arranged again. You can change the interval with **Check every** on the **Grid** tab of **Settings...** in the system tray menu, from 1.0 to 5.0 seconds in steps of 0.1 second.

### After you change the display scale, restart TwoTile

If you change the display scale while TwoTile is running, text in Settings and other windows looks blurry. Arranging isn't affected.

Select **Exit** in the system tray menu, and then start TwoTile again.

### Logs aren't saved to a file

TwoTile keeps its log only in the app, and the log is gone when you exit. When you contact support, copy it from the debug view before you exit ([How to Collect Logs](log_collection.en.md)).

### The portable version shows a warning the first time you run it

That's because it isn't signed. Select **More info**, and then **Run anyway**. It can't run on PCs where Smart App Control is on. Use the Store version.

### The Store version exits when it's updated

When the Microsoft Store updates TwoTile, the running TwoTile exits and doesn't start again on its own. Windows aren't arranged until it starts again. Start it from the Start menu, or it starts the next time you sign in (if you've set it to start with Windows). Your settings, and whether it starts with Windows, are kept after the update.

### The Store version's tray icon is hidden after an update

If you kept the TwoTile icon on the taskbar, it goes back into the list that opens from the ^ button on the taskbar after the Microsoft Store updates TwoTile. Windows remembers whether to show an icon for each app location, and the Store version's location changes with every update.

To show it again, turn on TwoTile in Windows Settings > Personalization > Taskbar > Other system tray icons. You can also drag the icon from the list to the taskbar. The portable version stays visible if you replace `TwoTile.exe` with the new version in the same place.

### If you install both versions, only one runs

If you install both the Store version and the portable version on the same PC, only the one you start first runs. The one you start later exits without showing a message.

## Tested environments

We've tested the Microsoft Store version and the portable version on the author's PC (Windows 11 Home 25H2, 64-bit, x64), with one and two displays, main display resolutions of 2560x1440 and 1920x1080, and display scales of 100%, 150%, and 200%.

The table below shows the status of other environments. "Not tested" means we haven't tested it yet.

| Environment | Status |
|:---|:---|
| Windows 10 | Not tested |
| Versions of Windows 11 other than 25H2 | Not tested |
| ARM PCs | Not supported |
| 32-bit Windows | Not supported |
| Three or more displays | Not tested. Windows on displays other than the main display should be left out in the same way |
| Different display scales on each display | Not tested |
| Display scales such as 125% and 175% | Not tested (100%, 150%, and 200% are tested) |
| Ultrawide and 4K displays | Not tested (the grid calculation is tested) |
| Rotated (portrait) displays | Not tested |
| Remote Desktop and virtual machines | Not tested |
| PCs where several users are signed in at the same time | Not tested |
| Installed from the Microsoft Store | Tested: starting and running in the system tray, where settings are stored, starting at sign-in, and keeping your settings and whether it starts with Windows when you update manually in the Microsoft Store app (from 1.0.1 to 1.0.2). **Automatic updates by the Store aren't tested** |
