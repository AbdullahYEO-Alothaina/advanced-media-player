# Changelog

All notable changes to the **Advanced Media Player** project will be documented in this file.

## \[3.2.2] - 2026-07-01

### Added

* Added an option in **Options > Audio Settings** to select the specific audio output device (sound card) for playback.
* Enabled switching sound cards instantly on-the-fly during active playback without needing to restart the player.
* Combined the check for application updates and YouTube updates into a single **Check For Updates** option.
* Optimized file searching inside directories to keep the player smooth and fast, even when searching through folders with thousands of files.
* Optimized file search/filtering inside the searchable files list dialog by running filtering on a background thread, debouncing text entry changes (250ms delay) to prevent redundant thread spawns, and limiting UI list rendering to the top 1000 items (with playing file auto-appended) to eliminate native control rendering lag.
* Added an **Info** submenu containing **About the Program** (which queries latest version info from GitHub in the background) and **Contact** (giving email and direct Telegram links).

### Removed

* Removed the separate and redundant "Check yt-dlp Updates" menu option and shortcut.
