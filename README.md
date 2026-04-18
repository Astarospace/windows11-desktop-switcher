### Quick note
I've tried the searene's windows-desktop-switcher script on my machine, on Windows 11. A bug would happen where the numbering will start from the current desktop instead of desktop 1. So, if I was on desktop 3, the numbering would start from there and I couldn't go to desktop 1 by pressing Win+1. This fork fixes this bug. 

Here's searene's quick note: I wrote this as a quick evening script to solve my problem. If you're looking for something more robust & need more than this script can give you, check out:
https://github.com/sdias/win-10-virtual-desktop-enhancer

# windows11-desktop-switcher
An AutoHotKey script for Windows 11 that lets a user change virtual desktops by pressing Win + &lt;num>. It also allows for creation/deletion of desktops by hotkey (see below).

## Overview
This script creates 'better' hotkeys for switching virtual desktops in windows 11. I built this to better mirror
the mapping I use on linux (with dwm), and it's always annoyed me that Windows does not have better
hotkey support for this feature (for instance, there's no way to go directly to a desktop by number).

## Installation
1. Install AutoHotKey.
2. Click on the green "Code" button.
3. Download the zip file.
4. Unzip the file.
5. Open autoHotKey Dash.
6. Click on "Compile".
7. At "Source (script file)", click browse.
8. Choose desktop_switcher.ahk script.
9. At "Base File (.bin, exe)", choose v1.1.37.02a0 U32 Ahk2Exe.exe (AutoHotKey will likely prompt you to install this version while trying to compile this script).
10. Press Convert

<img width="727" height="508" alt="image" src="https://github.com/user-attachments/assets/7d520caf-1ebb-436c-babd-50d338ab92af" />
<br><br>

* I would recommend putting it in your startup folder, the steps to do so are:
1. Right click on the desktop_switcher.exe
2. Click on "Create Shortcut".
3. Cut the shortcut file.
4. Click Win+R
5. Type shell:startup, and press enter.
6. Paste the shortcut file.

## Hotkeys
        <Win> + <Num>      - Switches to virtual desktop "num".
        <Win> + A or N     - Switch to virtual desktop on left
        <Win> + S or P     - Switch to virtual desktop on right

To change the key mappings, modify the bottom of the script and reload. Be sure to read about the [symbols AutoHotKey uses](https://autohotkey.com/docs/Hotkeys.htm) for key mapping.

## Other
To see debug messages, download [SysInternals DebugView](https://technet.microsoft.com/en-us/sysinternals/debugview).
