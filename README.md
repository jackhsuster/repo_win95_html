# Windows 95 Web OS (Single-File)

A standalone HTML/CSS/JS recreation of the Windows 95 desktop experience.  
Built with ES6+ OOP classes and zero external dependencies.

## Features
- OOP architecture: `WindowManager`, `Desktop`, `Taskbar`, `StorageManager`, `AppWindow`, `AppRegistry`.
- Windows: draggable, resizable (bottom-right handle), z-index focus, minimize/maximize/close.
- Taskbar: Start menu with nested items and active window buttons.
- Desktop: double-click icons to open apps, right-click custom menu.
- Apps:
  - **Notepad** with auto-save to `localStorage`.
  - **Command Prompt** with `help`, `ver`, `date`, `cls`.
  - **My Computer** (static display).
  - **小算盤** with +, -, *, /, memory (MC/MR/M+/M-), and keyboard input.
  - **Control Panel** (sound toggle).
- Optional click beep via Web Audio API.
- No CSS transitions (instant interactions).

## Usage
1. Open `index.html` directly in a modern browser (no build step).
2. Double-click desktop icons to launch apps.
3. Right-click on empty desktop for the context menu.
4. Use the Start button to open the Start menu.

## Data Persistence
Local data is stored under the `win95:*` prefix in `localStorage`.
- Notepad content: `win95:notepadContent`
- Sound toggle: `win95:soundEnabled`

To reset settings, clear site data or remove these keys in DevTools.

## Tech Stack
Pure HTML + CSS3 + Vanilla JavaScript (ES6+). No frameworks, no CDNs.
