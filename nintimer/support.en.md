---
layout: page
title: Support
lang: en
---

This applies to Nintimer 1.0.1 (public beta).

## How to contact us

The support contact, shared by all software made by poola-vii, is <https://github.com/poola-vii/support>. **Make it clear that you're writing about Nintimer.**

| What | How to send it |
|:---|:---|
| Bug reports, questions, and requests | Post from **Issues** in the repository, using one of the forms. **You need a GitHub account to post** (it's free) |
| Security vulnerabilities | Send them through **Private Vulnerability Reporting** on the **Security** tab of the repository. **Don't post them in a public issue** |
| Feedback you wrote in a Microsoft Store review | When we notice it, we'll reply publicly and point you to this contact, because Store reviews don't allow one-to-one conversations |

**You can contact us in English or Japanese.** Replies to questions in English may take longer than replies in Japanese.

### Don't include

Anyone can read public issues. Don't include:

- **Personal information**, such as names, addresses, phone numbers, email addresses, or employers
- **The content of your presentation**, such as slide titles or text, or anything that shows where or to whom you presented. If you attach a screenshot, hide the slide
- **Credentials**, such as passwords, tokens, or API keys
- **Undisclosed security vulnerabilities**. Use Private Vulnerability Reporting instead

If we find a post that includes any of these, we may edit or delete it.

### Please include

With these three things, we can usually look into the problem:

- **What you did and what happened.** Step by step, if you can. Also tell us which presentation app you used, and whether a full-screen slide show was running.
- **The Nintimer version.** It's at the top of the menu that opens when you right-click the timer or the system tray icon (for example, `Nintimer v1.0.1`). Also tell us whether you use the Microsoft Store version or the portable version.
- **The Windows version.** Edition, Version, and OS build, under Settings > System > About.

It also helps to know how many displays you use, and the resolution and scale of each (Settings > System > Display).

## How to collect the log

Nintimer writes a record to a file only **when it moves the timer automatically** (for example, when you disconnect a display or change the resolution and the timer would otherwise be off screen) and **when it gives keyboard input back to your slide show or other app after you use the timer's menu, Settings, or other windows**. It also writes one line at startup if it can't show the tray icon, or if it can't set up the notifications about foreground window changes that it uses to give keyboard input back. It doesn't record timing.

If the timer disappeared, moved somewhere unexpected, or your slides stopped advancing after you used the menu or Settings, include this file:

1. In File Explorer, type `%APPDATA%\nintimer` in the address bar and open it.
2. Open `nintimer.log` in Notepad, and paste its contents into your post. It contains only dates and times, the positions and sizes of the timer and displays, and the ID number of the window keyboard input was given back to (just a number, without window titles or contents) and whether that succeeded.
3. If the file doesn't exist, none of these has happened. That's a useful clue, too.

If you use the **Microsoft Store version** and there's no `nintimer` folder in that location, Windows has redirected it. In File Explorer, type `%LOCALAPPDATA%\Packages` in the address bar and open it. Then open the folder whose name contains `Nintimer`, and look in `LocalCache\Roaming\nintimer`.

You usually don't need to send the settings file (`config.json`). We'll ask for it if we need it.

## What we support

### What we do

- Investigate bugs in the latest version released as the public beta
- Answer questions about how to use it
- Keep the known issues up to date
- Fix the problems we decide to fix (in the next version)

### What we don't do

These are things **we can't do**. They don't mean we take your report lightly.

- **Support older versions.** Check whether the problem also happens in the latest version first.
- **Support for environments we've decided not to support.** ARM PCs, 32-bit Windows, and operating systems other than Windows.
- **Change behavior listed under "By design" in the known issues.** We chose it for a reason. We're still happy to hear your feedback.
- **Integrate with specific presentation apps.** Nintimer only stays on top of the screen. It doesn't connect to presentation apps.
- **Phone or in-person support.**

### What we can't promise

**The public beta is made by an individual in their spare time and distributed free of charge.**

- **We can't promise how quickly we'll reply.** It may take days or weeks.
- **We can't promise to act on every report.** We may decide not to fix something. If so, we'll tell you why.
- **We can't promise to keep distributing it.** We may stop. If we do, we'll announce it on the distribution site.
- **Behavior may change without notice during the public beta.** We'll list major changes in the [changelog](CHANGELOG.en.md).

For details, see the [Terms of Use](terms.en.md).
