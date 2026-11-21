---
layout: page
title: Known issues
lang: en
---

These are the known issues in HamonPlayer 1.0.1 (public beta), and the environments where it has been tested.

If you notice anything, let us know through the [support contact](support.en.md). We'll add what we learn to this page.

## By design

These behaviors are intentional, and we don't plan to change them.

### No shuffle

If you do nothing, every song comes back after about the same number of songs. When you skip a song, it takes longer before it plays again. Songs you Like come back sooner. There are no settings to order songs or to choose how they play. There are no playlists and no equalizer either.

### No main window

When HamonPlayer starts, it only shows an icon in the system tray. You start everything by clicking the icon and using its menus. Windows sometimes puts the icons of new apps in a hidden list. Open the "^" in the system tray to find it, and drag it to the taskbar to always show it.

### No notification pop-ups

Messages appear in the tooltip when you point at the icon. If a problem stops playback, the icon turns red, and the tooltip shows why.

### HamonPlayer pauses when another app plays sound

When another app plays sound for 2 seconds, HamonPlayer pauses, and the icon turns orange. When the other app has been quiet for 5 seconds, it plays again. Short notification sounds don't pause it. If you select Play yourself, it keeps playing even while the other app plays sound. To turn this off, clear **Pause when another app plays sound** on the **General** tab in **Settings…**. You can change the timing, and choose apps that shouldn't pause it (**Apps to ignore**), on the **Advanced** tab.

### HamonPlayer doesn't start playing when many songs are missing

At startup, if more than half of the songs in your play data can't be found, HamonPlayer doesn't start playing, and the icon turns red. This keeps your play data from becoming uneven, for example when an external drive isn't connected and only the other songs would play. If that's fine, right-click the icon and select **Start playing anyway**. The play data of missing songs is kept, and when they come back, they play with the same play data.

### The queue isn't saved

Songs you added to the queue are cleared when you exit HamonPlayer. The current song continues where it stopped the next time HamonPlayer starts.

### HamonPlayer doesn't change your song files

HamonPlayer only reads your song files. It doesn't change their tags or delete them. If you delete a file from your music folder, the play data for that song is kept, and if you put the same song back, it plays with its earlier play data.

### The Previous key isn't used

To hear a song that already played, add it to the queue from **History** in the search window.

### Two display languages: English and Japanese

HamonPlayer appears in Japanese when the Windows display language is Japanese, and in English otherwise. You can also choose the language with **Language** on the **Advanced** tab in **Settings…**. The change applies after you restart HamonPlayer. Other languages aren't available. Parts that Windows draws, such as the buttons in message boxes, appear in the Windows display language. Song names and artist names aren't translated.

**On Japanese Windows**, HamonPlayer appears in Japanese at first. To switch to English, right-click the icon and select **設定…** (Settings; the third item from the bottom). Open the **詳細** tab (Advanced; the tab on the right), set **言語** (Language) at the top to **English**, and select **OK**. Then right-click the icon, select **終了** (Exit; the last item), and start HamonPlayer again.

### No internet connection, no update notices

HamonPlayer doesn't connect to the internet, and it doesn't tell you when a new version is available. The Microsoft Store keeps the Store version up to date. For the setup.exe version, check the distribution site (https://github.com/poola-vii/HamonPlayer-releases ).

The only exception: when you turn on **Allow syncing to your phone** on the **Phone sync** tab in **Settings…**, HamonPlayer talks to your phone inside your home network (off by default; for details, see the [Privacy Policy](privacy_policy.en.md)).

## Things to watch out for

### The Microsoft Store version may close when the Store updates it

When the Microsoft Store updates HamonPlayer, the running HamonPlayer may close. It doesn't start again on its own, so the music stays stopped. Start it again from the Start menu.

If you want a version that doesn't change until you replace it yourself, you can use the setup.exe version instead.

### Install only one: the Store version or the setup.exe version

- You can't run both at the same time. The one you start second closes right away without doing anything.
- If you install the Store version on a PC where you used the setup.exe version, the Store version uses the same play data (`%LOCALAPPDATA%\HamonPlayer`).
- To switch from the Store version to the setup.exe version, export your play data in the Store version, uninstall it, and then import the file during first setup of the setup.exe version.

<!-- TODO: This was checked with the Store version registered in Developer Mode (2026-11-14, acceptance step A44). Check again with the version installed from the Store (T118) -->

### Before you connect a phone, phone sync listens on any network

Your PC remembers the networks where your phone has synced as home networks, and it doesn't listen on other networks. But until you connect a phone, and while the **Phone sync** tab in Settings is open, your PC listens on any network, even an outside one such as at a café or at work. A new phone needs the 6-digit code shown on your PC to connect, and your PC sends songs and play data only to phones you have connected.

<!-- threat_model.md C-4 (backlog T125, idea 1). From 0.1.60, HamonPlayer listens only on home networks -->

### Uninstalling the Store version also deletes your play data and settings

Windows keeps the play data and settings that the Store version makes in a place only for that app, so uninstalling deletes them. (On a PC where you used the setup.exe version first, the Store version uses `%LOCALAPPDATA%\HamonPlayer`, so they stay.)

The Store version backs up your play data to `HamonPlayer\backups` in your Documents folder, so the backups stay after you uninstall. When you install it again, your play data comes back from the newest backup after first setup. Changes after the last backup, your settings, and your connected phones do not come back.

To keep everything, before you uninstall, export your play data with **Export play data…** on the **Advanced** tab in **Settings…**. After you install it again, choose that file in **Import play data** during first setup.

<!-- TODO: This was checked with the Store version registered in Developer Mode (2026-11-14, acceptance step A44). Check again with the version installed from the Store (T118) -->

### The setup.exe version shows a warning the first time you run it

This is because it isn't signed. Select **More info**, and then select **Run anyway**. On PCs with Smart App Control turned on, you can't use it. Use the Microsoft Store version instead.

### At first, backups are on the same disk as your play data

HamonPlayer backs up your play data each time it starts, and before the first save of each day. At first, the backups are kept in the same place as your play data (`%LOCALAPPDATA%\HamonPlayer\backups`), so if the disk fails, you lose both. We recommend setting **Backup folder** on the **Advanced** tab in **Settings…** to another drive, or to a folder synced by OneDrive or a similar service.

### Files that can't play are skipped

Files that Windows can't play (damaged files, or files in a format Windows can't play) are skipped as songs that can't play, and are written to the log. Like a song you skip, such a song comes back less often.

### HamonPlayer may keep pausing and playing

If an app plays sound along with HamonPlayer, HamonPlayer may pause and play again every few seconds. After this happens 3 times with the same app, HamonPlayer stops watching that app and keeps playing. It keeps ignoring that app after HamonPlayer restarts, as long as the app is still running. While it isn't watching, it doesn't pause even when that app really plays sound. The tooltip shows "Auto-pause ignores <name> (it plays along with HamonPlayer)." To fix this, exit that app and start it again. If that doesn't help, add the app's process name to **Apps to ignore** on the **Advanced** tab in **Settings…**.

### "Safely remove" may not work for an external drive

This is because HamonPlayer watches your music folders to load songs you add. Before you remove the drive, exit HamonPlayer, or clear **Load new songs without restarting** on the **Advanced** tab in **Settings…**.

### In network folders, new songs may not be added right away

Changes in network folders may not be reported to HamonPlayer. In that case, new songs are added the next time HamonPlayer starts.

## Tested environments

We tested the setup.exe version by using it every day on our own PC (Windows 11 Home, 64-bit, x64). The music folders have thousands of songs, including music (wma, mp3, m4a, and aac) and videos (mp4 with H.264 video and AAC audio). Our own music folders have no flac songs, so we tested flac with files we made for testing. We tested on one display at 100% and 150% scale. We tested the English display with **Language** in **Settings…** set to English.

<!-- TODO: After T118 (acceptance step A44) checks the Store version, add what was checked here (installing, where the play data is kept, starting with Windows, whether only one copy runs). When you add a tested environment, update every sentence that lists tested environments in docs/public to the same content (rule in Nintimer's README) -->
