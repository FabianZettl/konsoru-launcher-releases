# KONSORU Launcher

<div align="center">

**A native Android HOME-replacement for the AYN Thor, with a bespoke themed UI per emulated console.**

[![Platform](https://img.shields.io/badge/platform-Android-3DDC84.svg?logo=android&logoColor=white)](https://www.android.com/)
[![Discord](https://img.shields.io/badge/Discord-Join-5865F2.svg?logo=discord&logoColor=white)](https://discord.gg/XSmG3crde9)
[![Ko-fi](https://img.shields.io/badge/Ko--fi-Support-FF5E5B.svg?logo=ko-fi&logoColor=white)](https://ko-fi.com/hollywoodkills)

[Download](../../releases/latest) · [Discord](https://discord.gg/XSmG3crde9) · [Ko-fi](https://ko-fi.com/hollywoodkills) · [Feedback](../../discussions)

</div>

## ⚠️ Early public feedback build — not a finished product

This is a first public release of KONSORU, shared specifically to get it in front of real AYN Thor
owners and collect feedback. It is **not** feature-complete and **will** have rough edges — see
[Known issues](#known-issues) below. If something looks broken, feels off, or an emulator won't
boot a game for you, please tell us on [Discord](https://discord.gg/XSmG3crde9) or open a
[discussion](../../discussions) — that's exactly what this release is for.

No source code is published in this repository — this is a binary-only release for testing and
feedback.

## About

KONSORU replaces your AYN Thor's homescreen entirely. Instead of one generic list for every
system, each emulated console gets its own themed shelf — inspired by the "Flat and Classic Mini
Consoles" LaunchBox BigBox theme — with console-appropriate backgrounds, selection styles, fonts,
and (where available) menu/navigation sound effects.

The Thor's second screen is used too: while you browse a console's game list on the main screen,
the lower screen shows live details and cover art for whatever's currently highlighted — and for
Nintendo 3DS specifically, the roles flip to match the real hardware (icon grid on the bottom
screen, Clear Logo art on top).

## Features

- Native Android HOME replacement — boots straight into KONSORU on the Thor
- Bespoke per-console themed shelves: Nintendo Switch, GameCube, Wii, Wii U, Nintendo 3DS
  (dual-screen aware), PlayStation 2, PSP, SNES/Classic-Mini style, Dreamcast
- Every other platform currently falls back to a clean generic grid
- Dual-display aware second-screen details view, matching the Thor's own hardware layout
- Cover art and metadata fallback via SteamGridDB and IGDB when local scraped data is missing
- Per-platform emulator selection, with RetroArch core support for classic systems

## Known issues

- This is an early alpha — expect bugs, most notably around getting specific emulators to
  actually boot a game on some platforms; we're actively working through these
- Not every console has a bespoke theme yet — anything without one uses the generic grid for now
- Built and tested specifically against the AYN Thor; behavior on other Android devices/launchers
  is unverified

## Installation

1. Download the latest APK from [Releases](../../releases/latest)
2. On the Thor, allow installing apps from the source you downloaded it with (Android will prompt
   you the first time if it's not already allowed)
3. Install the APK
4. On first launch, KONSORU will ask you to pick your ROM folder, then walk you through the rest
   of setup

To make KONSORU your default Home app, press the physical Home button and choose it when Android
asks, or set it manually under Android's own Home app settings.

## Feedback & support

This release exists to collect feedback — bug reports, impressions, platforms you'd like themed
next, anything. Please don't hold back.

- **Discord**: [discord.gg/XSmG3crde9](https://discord.gg/XSmG3crde9) — bugs, feedback, general chat
- **Support the project**: [ko-fi.com/hollywoodkills](https://ko-fi.com/hollywoodkills)
- **Bug reports / feature requests**: [GitHub Discussions](../../discussions) on this repo
