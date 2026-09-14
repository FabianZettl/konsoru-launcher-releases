# Changelog

All notable changes to KONSORU Launcher are documented here.

## v0.1.2

### New

- Single Screen Mode (Settings → Display) — for devices with only one screen: nothing gets
  launched on a second display, and 3DS shows its interactive grid directly on the main screen
  instead of splitting across two
- Switch UI sounds — navigation and launch confirm sounds, matching every other themed platform
- A short confirmation sound when backing out of a screen on the home shelf
- GB/GBC/GBA second-screen details reworked into one shared "paused retro RPG" style, each with
  its own accurate palette, instead of separate per-platform screens
- DPI/scaling fixes across GB/GBC/GBA and friends, so layouts hold their proportions correctly
- Onboarding: the soft keyboard no longer covers the Continue/Skip buttons while typing a
  SteamGridDB key

## v0.1.1

### New

- In-app update checker (Settings → Updates), with a Stable/Include-prereleases toggle and direct
  APK download link
- Options popups redesigned: one landscape, tabbed popup per platform (Startup Video / UI Sounds /
  Emulator), plus a new per-game popup (West/X on a focused game) for emulator override, manual
  metadata re-scrape, and manual cover/description swap
- UI Sounds toggle now actually mutes sounds, instead of being decorative
- Cover art on the generic (untheduled) platform grid, instead of blank tiles
- Device silhouette art behind each platform tile on the home shelf
- Cartridge insertion animation on launch for SNES/GBA/GB/GBC — the case slides out, centers
  full-screen, then flies into the console slot before the game boots
- Second-display watchdog: auto-relaunches the Thor's lower screen if it goes dark on its own
- One-time battery-optimization exemption prompt, to reduce background app kills

### Fixed

- 3DS crash on open (missing manifest entry for the interactive grid activity)
- 3DS emulator detection now recognizes Lime3DS, not just Azahar
- 3DS grid resized to match real hardware proportions; tooltip now spans all 3 visible tiles
- 3DS layout editor: tooltip bubble and text are now independently movable
- 3DS display desync on leaving the shelf via the grid's own back action
- Manual metadata/asset overrides were silently ignored when ES-DE data already existed — they now
  always take priority
- Options popups could get stuck showing the first platform/game opened (Koin ViewModel caching)

### Diagnosed, not yet resolved

- Wii U (Cemu): fails for "extracted" folder-format titles with no bootable file at the expected
  path — a ROM-scanning gap, not an emulator bug
- PS2 (ARMSX2): launches but the game doesn't visibly boot — cause still unconfirmed

## v0.1.0 — first public feedback build

Initial public release.

- Per-console themes: Switch, 3DS (dual-screen), GameCube, Wii, Wii U, Dreamcast, PS2, PSP, SNES —
  everything else uses a generic grid for now
- Second screen shows live game details/cover art; 3DS swaps screen roles to match real hardware
- Boot-menu music pauses correctly when the app loses focus; full-screen immersive shelf
- Per-platform emulator launching (Eden, Dolphin, Cemu, PPSSPP, ARMSX2/NetherSX2, Lime3DS/Azahar/
  Citra) plus RetroArch core support — not every listed emulator confirmed working yet
- Local ES-DE metadata/media support, with SteamGridDB/IGDB fallback
- Fixed: Wii U grid clipping/selection-jump, background color picker crash, 3DS grid sync and
  sizing
