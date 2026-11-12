# WinKlok

**A calmer, smarter clock mod for Windows 11 taskbar.**

WinKlok gives the Windows 11 taskbar clock a little more to do. Click the date/time area to open a native, Fluent-inspired panel for your calendar, stopwatch, timers, alarms, notes, and settings—with live stopwatch and timer previews beside the clock.

Windows' built-in clock is perfectly good at telling you the time. The rest of the job, apparently, was left as an exercise for the user.

## Quick links

<table style="margin-left: auto; margin-right: auto; border-collapse: collapse; text-align: center; font-family: sans-serif;" align="center">
  <tbody>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 10px 20px; font-weight: bold;">Use WinKlok</td>
      <td style="padding: 10px 20px;"><a href="https://windhawk.net/mods/winklok" target="_blank">Open the WinKlok page on Windhawk</a></td>
    </tr>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 10px 20px; font-weight: bold;">Get Windhawk</td>
      <td style="padding: 10px 20px;"><a href="https://windhawk.net/" target="_blank">Download Windhawk</a></td>
    </tr>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 10px 20px; font-weight: bold;">Source code</td>
      <td style="padding: 10px 20px;"><a href="https://github.com/shifting-whistler/WinKlok/blob/main/WinKlok.wh.cpp" target="_blank">Read <code>WinKlok.wh.cpp</code></a></td>
    </tr>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 10px 20px; font-weight: bold;">GitHub repository</td>
      <td style="padding: 10px 20px;"><a href="https://github.com/shifting-whistler/WinKlok" target="_blank">shifting-whistler/WinKlok</a></td>
    </tr>
    <tr style="border-bottom: 1px solid #ddd;">
      <td style="padding: 10px 20px; font-weight: bold;">Issues and suggestions</td>
      <td style="padding: 10px 20px;"><a href="https://github.com/shifting-whistler/WinKlok/issues" target="_blank">Report a bug or suggest an improvement</a></td>
    </tr>
    <tr>
      <td style="padding: 10px 20px; font-weight: bold;">License</td>
      <td style="padding: 10px 20px;"><a href="https://www.gnu.org/licenses/gpl-3.0.html" target="_blank">GNU General Public License v3.0 or later</a></td>
    </tr>
  </tbody>
</table>


## A look at WinKlok

### 1. The full desktop

<p align="center">
  <img src="Images/desktopv1.2.0.png" alt="WinKlok open on the Windows 11 desktop" width="100%">
</p>

### 2. Right there on the taskbar

Ever felt tired of moving those bulky floating panels just for a stopwatch or timer ? No worries, now they are displayed directly on the taskbar.

<table align="center">
<p align="center">
  <img src="Images/modetable.jpg" alt="WinKlok open on the Windows 11 desktop" width="100%">
</p>
</table>

### 3. Inside the panel



<table>
  <tr>
    <td width="33.33%"><img src="Images/rowfirst.png" alt="panel row 1" width="100%"></td>
 </tr>
 <tr>
  <td width="33.33%"><img src="Images/rowtwo.png" alt="panel row 2" width="100%"></td>
 </tr>
 <tr>
  <td width="33.33%"><img src="Images/rowthree.png" alt="panel row 3" width="100%"></td>
 </tr>

</table>

## What it does

### Calendar
* Month, year and decade views, with smooth vertical month scrolling like the Windows calendar.
* Today and the selected date are marked with your accent colour.
* **Events**: a thin ring of coloured segments around every date that has events, a hover card (up to five events, then "+N more"), and a double-click editor with all-day, start/end, title, description, location and colour.
* **Local mode**: any number of local calendars (with a protected *WinKlok (default)* calendar), import of Google Takeout ZIPs, `.ics` files and iCalendar links (duplicate-safe, edits are kept), and `.ics` export.
* **Google Calendar Sync mode** (Settings > Calendar settings): two-way sync with your own Google Cloud OAuth Desktop client. Local and Google data are kept completely separate. Calendars you own can be deleted (the primary one can be emptied) from the same page; this needs the full `calendar` scope, see the Help section there.
* Week numbers sit in a narrow column on the left and can be switched off in Calendar settings. The first day of the week and the first week of the year follow your Windows regional settings (no hard-coded ISO or Sunday rules).

### Stopwatch
* Centisecond precision, up to 200 laps (the newest lap is always on top) and a smooth lap list.
* Keeps running while the panel is closed and shows a live preview next to the clock.

### Timer
* Hours / minutes / seconds pickers, optional timer names and one-click presets you can save and remove.
* Run several timers at once. The most recently touched timer is shown beside the clock.

### Alarm
* Repeat on any days, custom label, snooze length and one of nine built-in sounds with live audition.
* The sound and snooze length you pick become the defaults for your next alarm.
* If an alarm or timer came due while the PC was off or asleep, it never rings late. One popup lists
  everything you missed, with dates and times.

### Tasks
* A minimal task list: **+** drops down the input (cursor ready, Enter adds), the trash icon deletes all tasks (two clicks to confirm).
* Slim cards with the date and time each task was created; edit or delete a task from its card.
* View: All / Active / Done. Finished tasks sink under a dimmed *Completed tasks* heading with its own Delete button.

### Notification panel
* The taskbar bell opens WinKlok's own notification panel instead of the Windows one: notifications grouped by app, relative times, dismiss one, dismiss a whole app, clear all, click to open the app.
* The icon can be left or right of the date and time, and can be always on, off, or shown only while there are notifications.
* In Settings > Notification settings choose **Separate panel** (the bell opens it on its own) or **Above WinKlok**: then the clock opens the WinKlok panel with the notifications stacked above it, sliding in from the right like the native flyout. A chevron in the tab bar folds the WinKlok panel into a slim strip so the notifications extend, and back (remembered).
* Notifications are read locally from the Windows notification database (read-only copy, nothing leaves your PC). If Windows ever blocks that, the panel says so and offers the native one.

### Notes
* Any number of notes, saved automatically, with a rich preview of Markdown and LaTeX maths.
* **Paste from ChatGPT, Gemini, Google and the web and keep the structure**: headings, lists,
  tables, block quotes, code blocks, links and equations are converted to Markdown as you paste.
* Links in the preview are clickable (only the link itself), plain URLs are detected automatically.
* One-tap **Copy** button for the whole note body (the title is not included), adjustable text size.

### Settings
* Settings is split into **General**, **Notification** and **Calendar** pages.
* General: taskbar previews, which tabs are shown (drag them to reorder), preview layout, 12/24-hour time (applied everywhere), panel material (acrylic or simple), default timer / alarm sounds and the **panel horizontal position**.
* The panel opens in the corner next to the clock (below the taskbar when the taskbar is at the top). The position slider moves it along the screen in single-pixel steps, up to the left edge (useful on ultrawide screens); the notification stack then rises from the taskbar instead of sliding in from the edge.
* **Sync time now** (Windows asks for administrator permission whenever it is needed).
* A compact **About** card with the version, developer, project links and a bug / feature request button.

### Taskbar integration and settings

- Native Win32, Direct2D, and DirectWrite rendering—no embedded browser UI.
- Acrylic or simple panel material, light/dark theme support, and Windows-style slide-up animation.
- Mouse-wheel, touch, pen, and precision touchpad scrolling.
- Optional taskbar previews and notification icon, configurable 12/24-hour display, preview layout, and default timer/alarm sounds.
- Controls to sync system time, reload Explorer/the taskbar, or quit WinKlok and return the clock area to Windows.

## Getting started

1. Install [Windhawk](https://windhawk.net/).
2. Open the [WinKlok mod page](https://windhawk.net/mods/winklok) and install/enable the mod through Windhawk. 
3. Restart the Windows Explorer from the task manager if changes don't appear.
4. Have fun...


## Tips
* Scroll over the tab bar to reveal more tabs, or click a tab to slide it to the centre.
* Right-click a timer preset to reveal its remove button.
* WinKlok always hides the Windows notification bell while it runs. Its own notification icon is optional: turn it off in Settings and, with *Above WinKlok*, the clock still opens the notifications together with the panel.

## Compatibility
* Windows 11 with the XAML taskbar, 64-bit only.
* Do not combine with other mods that rebuild the taskbar clock area (for example *Taskbar Clock
  Customization*) until you have verified they coexist.
* The panel always rests next to the taskbar (above a bottom taskbar, below a top one), even when it is set to auto-hide (it keeps clear of the area the taskbar occupies when shown).
* WinKlok does not change the taskbar height. Use the *Taskbar height and icon size* mod for that.
* To turn WinKlok off, disable the mod in Windhawk: the taskbar clock goes back to Windows immediately.
* If something misbehaves, enable logging for this mod in Windhawk and check the log.

## For developers
* Single-file C++ mod, organised in blocks: engine and persistence, taskbar integration (XAML
  injection and hooks), native UI primitives, sound synthesis, rich-text and LaTeX engine, panel
  pages and alert windows.
* Rendering is plain Win32 + Direct2D/DirectWrite. There is no browser engine and no external asset.
* Alarm sounds are synthesised at runtime into in-memory WAV buffers, so nothing needs to be shipped.
* The pasted-HTML to Markdown converter lives next to the Notes editor and understands the clipboard
  *HTML Format* produced by modern browsers and chat apps.
* Contributions, bug reports and ideas are welcome on GitHub.

## Contributing and support

Bug reports, compatibility notes, ideas, and pull requests are welcome in the [GitHub Issues](https://github.com/shifting-whistler/WinKlok/issues) and [repository](https://github.com/shifting-whistler/WinKlok).

Made by **Shifting Whistler**.

---

WinKlok is free and open-source software licensed under **GPL-3.0-or-later**. See the [full licence text](https://www.gnu.org/licenses/gpl-3.0.html) for the terms.

