---
layout: page
title: Changelog
lang: en
---

Dates are in Japan Standard Time. The Microsoft Store version and the setup.exe version share the same version numbers. This is the same as **Help** > **What's new** in the app, except for the dates: here each date is the release date, and in the app it's the date the version was built.

> **About version numbers.** Versions 0.x were used during development before release. The first released version is **1.0.2** (1.0.0 and 1.0.1 were not released). The beta status is shown on the download pages and in this document, not in the version number.

<!--
  How to write: Keep the content the same as What's new in the app (src/help/changes.en.html).
  When the first released version is built, also merge the pre-release entries in the in-app What's new into one entry like the 1.0.2 entry below (persona.md 5.2, item 1).
  Write the release date on the version line. A version may be built and not released (release.md 3.6).
  Don't write a date on the line of a version that was not released (tools/make-installer.ps1 treats the top version with a date as the released version. backlog T138).
  Add phone version changes with "Phone:" after the phone version is released.
-->

---

## 1.0.6 — Not released yet (the date goes in on the release day)

- In Help, "Terms and licenses" now shows this version as the version it applies to.

---

## 1.0.5 — Not released

**This version was not released.** Its changes are included in 1.0.6.

- With "Play videos full screen behind other windows", if the monitor with the video window is disconnected, videos now play in the small window instead of filling another monitor. When you connect it again, videos fill it again. Settings and Help now explain how to keep videos playing on a second monitor.
- Fixed the video window starting at the default small size instead of the size you set, when it was on a second monitor with a different Scale setting in Windows.

---

## 1.0.4 — Not released

**This version was not released.** Its changes are included in 1.0.6.

- The first sentence of "How to use" in Help now says "the songs you own" instead of "your own songs", which could be read as songs you wrote.

---

## 1.0.3 — Not released

**This version was not released.** Its changes are included in 1.0.6.

- The play data in "Info…" is simpler. It still shows "n songs since last play" and "Next in about n songs".

---

## 1.0.2 — 2026-11-22

The first released version (public beta).

- Just leave it running, and it keeps playing the songs in your music folders. It doesn't shuffle. Songs you skip take longer to come back.
- When you like what you hear, select Like, and the song comes back sooner.
- It pauses when another app plays sound, and plays again when the other app is quiet.
- Music and videos each play as one song. Video songs show in a small window.
- You can search for songs and add them to the queue. You can see the songs you just played in History.
- You can set a play schedule (start and stop times for each day of the week). It can start with Windows.
- It plays all songs at a similar volume.
- When you add songs, it loads them without restarting. Moved songs keep their play data.
- It backs up your play data every day, and you can restore it from a backup you choose. You can choose the backup folder. You can export your play data to one file and import it on a new PC.
- Menus, windows, How to use, the manual, What's new, and the installer are shown in English or Japanese.
- Available as the Microsoft Store version and the setup.exe version. Both are the same app.
