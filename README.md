# Desktop

A browser-based desktop environment prototype inspired by the macOS Tahoe visual language and the Linux MacTahoe theme projects.

## Run

Open `index.html` on a modern desktop browser. The SVG entrypoint is `osama.svg`; it embeds the same desktop interface for direct viewing in browsers that support SVG `foreignObject` and scripting.

## Included in this preview

- Tahoe-style desktop wallpaper with day/night variants
- Translucent menu bar, system status area, Dock and popovers
- Dock magnification that pushes neighboring icons aside, bounce feedback, running indicators, scrollable narrow-screen Dock, animated popovers, and window transitions
- Finder-style file manager with a populated Home directory, sidebar navigation, inline search, new folders, file selection, drag-and-drop moves, reordering, rename, duplicate, trash, preview, and context actions. File changes persist locally in the browser
- System Settings with appearance, wallpaper, Dock, desktop, Control Center, sound and keyboard sections
- Launchpad and Spotlight-style app search
- Control Center with Wi-Fi, Bluetooth, Focus, brightness, volume, Dark Mode and screen-mirroring toggles
- Notification Center widgets and live clock
- Browser, Messages, Notes, Calculator, Terminal, App Store, Music and Photos windows
- Draggable, resizable from edges and corners, focusable, minimizable and maximizable app windows
- Keyboard shortcuts: `Ctrl/⌘ + Space` for search, `F4` for Launchpad, `Ctrl/⌘ + N` for Finder, and `Ctrl/⌘ + W` to close the focused window

## What it is

This is a desktop UI prototype that runs inside a web browser. File contents, connectivity, power, sound and other hardware-level operations are simulated; it is not a bootable operating system or a replacement for a Linux desktop session.

## Theme references and assets

The visual direction references [MacTahoe GTK Theme](https://github.com/vinceliuice/MacTahoe-gtk-theme) and [MacTahoe Icon Theme](https://github.com/vinceliuice/MacTahoe-icon-theme).

The day/night wallpaper images are loaded from the MacTahoe GTK Theme repository. The application, folder, file-type, and Firefox SVG icons are loaded from the MacTahoe Icon Theme repository; no generated app icons are used. Their upstream license texts are included under `LICENSES/`. Other app glyphs in this prototype are custom inline SVG drawings.

- GTK theme and wallpaper source: MIT, see [LICENSES/MacTahoe-gtk-MIT.txt](LICENSES/MacTahoe-gtk-MIT.txt)
- Icon source: GPL-3.0, see [LICENSES/MacTahoe-icon-GPL-3.0.txt](LICENSES/MacTahoe-icon-GPL-3.0.txt)

## Project structure

- `index.html` — main desktop shell
- `osama.svg` — SVG-hosted copy of the desktop shell
- `browser.html` — Browser app loaded inside its desktop window
- `assets/icons/` — bundled upstream MacTahoe icon-theme SVG files
- `LICENSES/` — upstream theme license texts
