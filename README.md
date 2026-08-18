# anifuzz

<video src="https://github.com/user-attachments/assets/a9f53cca-d68a-4329-aba5-a9bdd2c08cb0" controls="controls" width="100%"></video>

A heavily stripped-down, GUI-first fork of [ani-cli](https://github.com/pystardust/ani-cli), optimized specifically for `fuzzel` and tiling window managers (Sway, Hyprland, etc.).

All terminal-specific baggage, redundant menus, and useless disk I/O have been ripped out to make it as fast and lightweight as possible.

## Requirements
- `mpv` (Video playback)
- `fuzzel` (Application launcher/menu)
- `curl`, `grep`, `sed` (Standard utilities)
- `ani-skip` (Optional: for skipping intro themes)

## Installation & Usage

### 1. The Script
Make the script executable and place it anywhere in your `$PATH` (like `~/.local/bin/`):
```bash
chmod +x anifuzz
mv anifuzz ~/.local/bin/
```

### 2. Desktop Entries (Application Launcher)
To make Anifuzz show up in your GUI application launcher, copy the provided `.desktop` files into your applications folder:
```bash
cp *.desktop ~/.local/share/applications/
update-desktop-database ~/.local/share/applications/
```

You can now search for **Anifuzz** or **Anifuzz (History)** straight from your launcher!

### 3. Keybinds (Optional)
Alternatively, you can bind these directly to your window manager shortcuts:
- Launch and search: `anifuzz`
- Resume from history: `anifuzz -c`

## Legal & License
This is a personal fork of `ani-cli`. All original scraping logic and architectural credit goes to the `ani-cli` contributors. 
Licensed under the GNU General Public License v3.0 (GPLv3).
