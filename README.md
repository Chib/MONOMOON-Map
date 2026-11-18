# 🌙 MONOMOON Map

A simple, unofficial map builder for MONOMOON. Paste screenshots of individual game screens into a seamless, zoomable grid, switch between aligned Outside and Inside maps, and add markers to remember important locations.

Everything runs locally in your browser. Your screenshots, markers and settings are saved in a folder you choose on your computer.

## Features

- **Screenshot mapping:** Paste a screenshot with `Ctrl+V`, then click the grid square where it belongs. Screenshots sit flush against each other, and existing tiles can be replaced or moved.
- **Expandable map:** Add screens in any direction, then pan and zoom to explore the assembled map.
- **Two aligned layers:** Switch between Outside and Inside without changing the map's position or zoom. Optionally show the other layer faintly as a reference.
- **Custom markers:** Add markers anywhere, including empty grid squares. Choose from six shapes and nine colours, add optional notes, and edit or move markers later.
- **Customisable display:** Toggle grid lines, markers, hints and interface buttons. Adjust keyboard pan speed, marker size and screenshot cropping.
- **Local saving:** Screenshots, marker details, map positions and display preferences are stored in your chosen local folder, with backup export and restore options.

## Getting started

1. Download the repository (click **Code → Download ZIP**) and extract it, or download `MONOMOON_Map.html` on its own.
2. Open `MONOMOON_Map.html` in **Google Chrome or Microsoft Edge** on your computer. No installation or web server is required.
3. When prompted, choose a folder to hold your map data. You can create a new, empty folder for this.
4. Take a screenshot of a game screen, press **Ctrl+V** on the map page, and click the grid square where it belongs.
5. Keep adding screenshots. Changes are saved to the selected folder automatically.

**Browser compatibility:** Direct saving to a local folder uses the File System Access API, which is supported in Chrome and Edge. **Firefox is not supported** for this folder-saving mode. Your browser may ask you to select or authorise your map folder again after reopening the page.

### Screenshot cropping

If your screenshots contain black borders or other areas that aren't part of the game screen, open **⋯ → Adjust screenshot crop** to set the left, right, top and bottom crop values. All screenshots use the same crop dimensions so neighbouring tiles line up correctly.

## Controls

| Action | Control |
| --- | --- |
| Paste a screenshot | `Ctrl+V`, then click a grid square |
| Pan the map | Click and drag, `WASD`, or arrow keys |
| Zoom | Mouse wheel or on-screen `+` / `−` buttons |
| Switch Outside / Inside | `Space` |
| Show / hide markers | `Ctrl+Space` |
| Toggle grid over screenshots | `G` |
| Add, move or delete a screenshot / marker | Right-click the map or marker |
| Save marker notes | `Ctrl+Enter` |
| Pick marker colour or shape | `Tab` to the palette, then use arrow keys |
| Save from a marker colour / shape palette | `Enter` or `Ctrl+Enter` |
| Cancel a placement, move or edit | `Esc` |

The **⋯** menu also provides display settings, screenshot crop controls, folder options and backup tools. You can choose to keep grid lines visible on empty tiles even when the grid overlay is switched off.

## Where your map is saved

MONOMOON Map saves your data in a **local map folder**, separate from the HTML file. A typical folder contains:

```text
MONOMOON Map Data/
├── map.json          # Map positions, markers and settings
├── outside/          # Outside screenshots
└── inside/           # Inside screenshots
```

Your map is **not embedded in the HTML file**. You can update or share the HTML without including your screenshots or settings. To share a particular map, you would need to share its map-data folder separately.

**Back up your map folder periodically**, especially before reorganising or deleting files. You can also use **⋯ → Export map backup**. If folder access is lost, reconnect it before continuing to edit; the app is designed to stop saving rather than silently switch to browser storage.

## Disclaimer

This is an unofficial, fan-made tool and is not affiliated with or endorsed by the creators of MONOMOON. Game imagery and other game-related assets remain the property of their respective owners.

### Development

MONOMOON Map was developed using OpenAI's ChatGPT. The project's design, features and functionality were directed and tested by the repository owner, with the application code largely generated through AI assistance and refined through iterative testing and feedback.

## Licence

The code is released under the [MIT License](LICENSE). You may use, modify and redistribute it under the terms of that licence.
