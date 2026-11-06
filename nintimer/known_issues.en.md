---
layout: page
title: Known issues
lang: en
---

These are the known issues in Nintimer 1.0.1 (public beta), and the environments where it has been tested.

If you notice anything, let us know through the [support contact](support.en.md). We'll add what we learn to this page.

## By design

These behaviors are intentional, and we don't plan to change them.

### Stop doesn't let you resume

When you select **Stop**, the value at that moment stays on screen in gray. If you then select **Start over**, the timer starts again **from zero, not from where it stopped** (from the full time limit, or from `00:00` when counting up). In Japanese, these menu items are 一時停止 and 開始.

These commands are for starting over when a presentation didn't actually start, and for reading how long a presentation took. There's no command to continue from where the timer stopped.

### Selecting OK in Settings restarts the timer

If you select **OK** in Settings while the timer is running or stopped, that timing is discarded, and the timer goes back to waiting with the new settings (when you use start and end times, the new time window starts right away). **This also happens when you change the display language.** Choose the language and appearance settings before your presentation.

### The audience can see the timer

The timer appears in a corner of the screen you're projecting. It's small and semi-transparent, but the audience can see it. To hide it, right-click the system tray icon and select **Hide overlay** (timing continues).

### Two display languages: English and Japanese

Nintimer appears in Japanese when the Windows display language is Japanese, and in English otherwise. You can also choose English or Japanese with **言語 / Language** at the bottom of Settings. Other languages aren't available. Parts that Windows draws, such as the buttons in message boxes, appear in the Windows display language.

**On Japanese Windows**, Nintimer appears in Japanese at first. To switch to English, right-click the timer or the system tray icon, select **設定...** (Settings; the only item that ends with three dots), set **言語 / Language** to **English**, and then select **OK**.

### No sound, no network, no update notices

Nintimer doesn't make a sound when time is up. It doesn't connect to the internet, and it doesn't tell you when a new version is available. The Microsoft Store keeps the Store version up to date. For the portable version, check the distribution site (https://github.com/poola-vii/Nintimer-releases ).

### Timing isn't saved

If you close Nintimer or restart your PC, the timing is lost, and Nintimer starts in the waiting state the next time. Your settings and the timer's position are kept.

## Things to watch out for

### The Microsoft Store version may close when the Store updates it

When the Microsoft Store updates Nintimer, the running Nintimer may close. If this happens during a presentation, the timer disappears.

The Store version's package declares that updates should be deferred while the app is in use. However, this declaration doesn't work on versions of Windows earlier than Windows 11 24H2, and we haven't confirmed that it works for Nintimer. We'll keep this issue listed until we have.

There are two ways to make sure Nintimer doesn't close during a presentation. Choose one:

- **Before the day of your presentation, pause app updates in the Microsoft Store.** In the Microsoft Store **Settings**, turn off **App updates**. The **Pause updates** window opens. Choose a **Pause duration** of 1 week, 2 weeks, 3 weeks, 4 weeks, or 5 weeks, and then select **Confirm** (Microsoft's article "Get updates for apps and games in Microsoft Store"). Turn updates back on after your presentation.
- **Use the portable version.** The portable version doesn't change until you replace the file yourself.

### If you install both the Store version and the portable version on one PC

- **Only the one you start first runs.** The one you start later closes without a message.
- **Whether the two share settings depends on the PC.** On a PC that has the `%APPDATA%\nintimer` folder (because you used the portable version first), both versions use the same settings. Otherwise, the Store version keeps its settings in its own location, separate from the portable version's. They're removed when you uninstall the Store version.

### The portable version shows a warning the first time you start it

This is because it isn't signed. Select **More info**, and then select **Run anyway**. On PCs with Smart App Control turned on, it can't start. Use the Microsoft Store version instead.

### Nintimer can't appear above some full-screen apps

The timer can't appear above apps that run in DirectX exclusive full-screen mode (some games and video apps). This is how Windows works. It does appear above normal full-screen slide shows.

### The "Terms, licenses, and download sources" window goes under the timer

The timer always stays on top, so it covers any part of this window that overlaps it. Move the window to read it.

## Tested environments

We tested the portable version and the Microsoft Store version on our own PC (Windows 11 Home, 64-bit, x64) with full-screen slide shows in LibreOffice Impress, on one display at 100%, 150%, and 200% scale. Before release, we installed the Microsoft Store version in developer mode to check how it shows over a full-screen slide show, that it starts, where it keeps settings, and that only one copy runs. We tested the English display with the language setting set to English, and with a user whose Windows display language is English (with that user, we didn't test it together with a full-screen slide show).

The table below shows the status of other environments. "Not tested" means we haven't checked it yet.

| Environment | Status |
|:---|:---|
| Windows 10 22H2 | Not tested |
| PowerPoint slide shows | Not tested (we expect the timer to stay on top the same way, but we haven't checked) |
| Different scales on different displays (for example, a laptop at 150% and a projector at 100%) | Not tested |
| ARM PCs, 32-bit Windows | Not supported |
| Installed from the Microsoft Store | Not tested (we'll check after release). Automatic updates from the Store are also not tested |
