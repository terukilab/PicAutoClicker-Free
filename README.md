# PicAutoClicker — Free Edition

An image recognition auto-clicker that finds and clicks images displayed on your screen.

[![Version](https://img.shields.io/badge/Version-0.9-orange)](https://github.com/terukilab/PicAutoClicker-Free/releases)
[![Platform](https://img.shields.io/badge/Platform-Windows%2011-lightgrey?logo=windows)](https://www.microsoft.com/windows)

---

## Overview

PicAutoClicker Free is a Windows desktop application that searches for target images on the screen using template matching and automatically clicks on them.

No programming required — everything is controlled through an intuitive GUI. It can be used for a wide range of purposes, including automating repetitive tasks and reducing manual effort on routine operations.

---

## System Requirements

| Item | Requirement |
|------|-------------|
| OS | Windows 11 (64bit) |
| Other | No additional installation required |

---

## Installation

1. Download `PicAutoClicker_free.zip` from the [Releases page](https://github.com/terukilab/PicAutoClicker-Free/releases)
2. Extract the ZIP to any folder
3. Double-click `PicAutoClicker_free.exe` to launch

No installer is needed. It is ready to use immediately after extraction.  
To uninstall, simply delete the extracted folder.

---

## Features

- Register images by capturing a region of the screen (just drag to crop)
- Image search using template matching
- Manage multiple projects with tabs
- Loop execution (repeat a specified number of times)
- Configure step wait and pre-click wait times
- Timeout setting (skip if image is not found; set to 0 for infinite wait)
- Confidence threshold adjustment with a slider
- Window-targeted search (limit the search area to a specific window)
- Reorder steps by drag and drop
- Real-time execution log
- Emergency stop via ESC key or mouse movement
- Japanese / English display language toggle

---

## How to Use

### Basic Flow

1. Create a new project tab with the `[+]` button
2. Click `✂ Capture` and drag to crop the area you want to click (multiple images can be registered)
3. Adjust the run settings in the left panel
4. Click `▶ Play` to start

### Run Settings

| Setting | Description |
|---------|-------------|
| Loop Count | How many times to repeat the image list |
| Step Wait | Wait time after each click (seconds) |
| Pre-click Wait | Wait time just before clicking (seconds) |
| Timeout | Seconds to wait before skipping if image is not found (0 = infinite) |
| Confidence | Matching threshold (lower values find more but increase false positives) |
| Target Screen | Fullscreen / Window-targeted |
| Stop Method | ESC key only / Any mouse or key input |

### Image List Operations

| Action | Method |
|--------|--------|
| Reorder | Drag and drop |
| Delete | 🗑 button |
| Replace image | Right-click → Replace image |
| Copy / Paste | Right-click → Copy / Paste |
| Play from here | Right-click → Play from here |

### Project Tab Operations

| Action | Method |
|--------|--------|
| Add tab | `[+]` button |
| Rename tab | Right-click tab → Rename |
| Duplicate tab | Right-click tab → Duplicate |
| Delete tab | Right-click tab → Delete |

---

## About Image Recognition

Template matching (OpenCV) is used for image recognition.

- The screen must be displayed at the same resolution and color tone as when the image was captured
- Lowering the confidence value makes images easier to find but increases false positives
- In Window-targeted mode, only the interior of a specific application window is searched

---

## Failsafe

Moving the mouse cursor to any corner of the screen will forcibly stop the automation.  
If unintended clicks continue, quickly move the mouse to a screen edge.

---

## Language Settings

You can switch between Japanese and English from the ⚙ button. A restart of the application is required after changing the language.

---

## Terms of Use / Disclaimer

- Redistribution of this software to third parties is prohibited.
- Modification, decompilation, and reverse engineering of this software are prohibited.
- The author assumes no responsibility for any damages or issues (including unintended clicks, data loss, or service account suspension) arising from the use of this software.
- Use of this software with services that prohibit automated operations is not allowed. Please comply with the terms of service of each platform.

---

## Author / Contact

terukilab

- GitHub: [@terukilab](https://github.com/terukilab)
- Bug reports and feature requests: [Issues](https://github.com/terukilab/PicAutoClicker-Free/issues)
