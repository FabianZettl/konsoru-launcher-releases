# Changelog

All notable changes to KONSORU Launcher are documented here.

## v0.1.0 — first public feedback build

Initial public release. Everything below is new, since this is the first version anyone outside
of on-device testing has seen.

### Per-console themes

- **Nintendo Switch** — tile row with the real Switch Home Menu chrome and selection glow
- **Nintendo 3DS** — built around the Thor's dual screens like the real hardware: an interactive
  icon row on the bottom screen, wobbling Clear Logo art for the highlighted game on the top
  screen
- **GameCube** — disc-menu-style shelf, with the console's own boot video and menu music
- **Wii** — Wii Menu-style channel grid
- **Wii U** — Wii U Home Menu-style tile grid with placeholder tiles, plus functional
  Settings/Shop/Browser utility tiles and a live background-color picker
- **Dreamcast** — swirl-menu-style shelf with its own boot video and UI sounds
- **PlayStation 2** — full coverflow-style case-browsing recreation
- **PSP** — XMB-style recreation
- **SNES** — Classic Mini-style boot shelf
- Every other platform uses a clean generic grid until it gets its own theme

### Dual-screen support

- The Thor's second screen shows live game details and cover art for whatever's highlighted on
  the main screen
- For Nintendo 3DS specifically, the two screens swap roles to match real 3DS hardware — the
  interactive grid lives on the bottom screen, Clear Logo art on top
- Background menu music now correctly pauses when the app loses focus (e.g. when an emulator
  launches) instead of continuing to play underneath it
- Full-screen immersive mode: both the status bar and gesture-navigation bar are hidden on the
  main shelf

### Emulator integration

- Per-platform emulator launching for Switch (Eden), GameCube/Wii (Dolphin), Wii U (Cemu), PSP
  (PPSSPP), PS2 (ARMSX2/NetherSX2), 3DS (Lime3DS/Azahar/Citra), plus RetroArch core support for
  classic systems
- Honest per-emulator "verified working" flagging under the hood — not every listed emulator has
  been confirmed to actually boot a game yet, see Known Issues in the README

### Metadata & cover art

- Local ES-DE-style metadata and media support (covers, screenshots, marquees/Clear Logos, etc.)
- SteamGridDB and IGDB fallback for cover art and descriptions when local data is missing

### Fixes since early internal builds

- Fixed the Wii U tile grid clipping behind its own background and the selected tile jumping out
  of the grid instead of just gaining a highlight border
- Fixed the Wii U background color picker crashing when sampling a color from screen
- Fixed the 3DS interactive grid and the top-screen details view falling out of sync when leaving
  the 3DS shelf
- Fixed 3DS tile sizing and spacing to match real 3DS hardware proportions
