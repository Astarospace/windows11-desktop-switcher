### Quick note
I wrote this as a quick evening script to solve my problem. If you're looking for something more robust & need more than this script can give you, check out:
https://github.com/sdias/win-10-virtual-desktop-enhancer

# windows11-desktop-switcher
An AutoHotKey script for Windows 11 that lets a user change virtual desktops by pressing Win + &lt;num>. It also allows for creation/deletion of desktops by hotkey (see below).

## Overview
This script creates 'better' hotkeys for switching virtual desktops in windows 11. I built this to better mirror
the mapping I use on linux (with dwm), and it's always annoyed me that Windows does not have better
hotkey support for this feature (for instance, there's no way to go directly to a desktop by number).

## Installation
Install AutoHotKey, then run the desktop_switcher.ahk script (open with AutoHotKey if prompted). I would recommend putting it in your startup folder and it'll be invoked on login.

## Hotkeys
        <Win> + <Num>      - Switches to virtual desktop "num".
        <Win> + A or P     - Switch to virtual desktop on left
        <Win> + S or N     - Switch to virtual desktop on right

To change the key mappings, modify the bottom of the script and reload. Be sure to read about the [symbols AutoHotKey uses](https://autohotkey.com/docs/Hotkeys.htm) for key mapping.

## Other
To see debug messages, download [SysInternals DebugView](https://technet.microsoft.com/en-us/sysinternals/debugview).

Notice: I've tried the original windows-desktop-switcher script on my machine, on Windows 11. A bug would happen where the numbering will start from the current desktop instead of desktop 1. So, if I was on desktop 3, the numbering would start from there and I couldn't go to desktop 1 by pressing Win+1. This fork fixes this bug.
