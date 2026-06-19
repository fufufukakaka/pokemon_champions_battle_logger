# Pokemon Champions Battle Logger

<p align="center">
  <img src="https://img.shields.io/github/v/release/fufufukakaka/pokemon_champions_battle_logger?style=flat-square&color=FF3B30" alt="Release">
  <img src="https://img.shields.io/github/downloads/fufufukakaka/pokemon_champions_battle_logger/total?style=flat-square&color=00B4DC" alt="Downloads">
  <img src="https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux-32D74B?style=flat-square" alt="Platforms">
  <img src="https://img.shields.io/badge/license-Proprietary-555?style=flat-square" alt="License">
</p>

<p align="center">
  <strong>Dominate Your Battle Data.</strong><br>
  Pokemon Champions Battle Logger automatically records and analyzes battles live or from recorded video.
</p>

> 🇯🇵 日本語版は [README.md](README.md) をご覧ください。

---

## Features

- **Live Scan** - Read an OBS Virtual Camera feed while you play, then log turns, HP, and active Pokemon automatically
- **Recorded Video Analysis** - Drop a YouTube URL or local video file to detect battles, recognize Pokemon, read moves, and determine win/loss
- **Singles and Doubles** - Battle logs, team selection, opponent teams, and usage stats work for both formats
- **In-Battle Assist** - Match the opponent's six Pokemon against top-ranker teams and past matchups, then check lines in the damage desk
- **Deep Analytics** - Win rate trends, team selection stats, knockout statistics, battle details, and notes in one dashboard
- **Language Support** - The app UI supports Japanese and English. Game text recognition supports Japanese, English, Traditional Chinese, Simplified Chinese, Korean, French, Spanish, Italian, and German
- **Local Records** - Battle records stay on your machine. Some OCR / AI features may use external AI APIs when configured
- **Free for Personal Use**

## Download

> **Latest Release**: [Download here](https://github.com/fufufukakaka/pokemon_champions_battle_logger/releases/latest)

| Platform | File |
|----------|------|
| Windows (x64) | `poke-champions-logger-windows-x64-setup.exe` |
| macOS (Apple Silicon) | `poke-champions-logger-macos-arm64.dmg` |
| Linux (x64) | `poke-champions-logger-linux-x64.deb` |

### Quick Start

1. Download the installer for your platform from [Releases](https://github.com/fufufukakaka/pokemon_champions_battle_logger/releases/latest)
2. Install / open the app (see platform notes below)
3. The app opens in your browser at `http://127.0.0.1:8000`
4. Follow the initial setup wizard (choose language, enter trainer name)

### Windows Users

Windows SmartScreen may display a **"Windows protected your PC"** warning when launching the app for the first time. This is because the executable is not code-signed (Windows code-signing certificates are prohibitively expensive for a personal project).

To run the app:

1. Click **More info** on the warning dialog
2. Click **Run anyway**

Some antivirus software may also flag the executable as a false positive. If this happens, please add an exception for `poke_champions_logger.exe`.

## Screenshots

### Dashboard

<p align="center">
  <img src="docs/dashboard.png" alt="Dashboard" width="800">
</p>

### Live Scan

<p align="center">
  <img src="docs/live_scan.png" alt="Live Scan" width="800">
</p>

### Analysis

<p align="center">
  <img src="docs/analysis.png" alt="Analysis" width="800">
</p>

### Battle Detail

<p align="center">
  <img src="docs/battle_detail.png" alt="Battle Detail" width="800">
</p>

## Requirements

- **Input**: 1920x1080 (1080p) 30fps recommended
- **Format**: Singles and doubles in Pokemon Champions
- **Live Scan**: OBS Virtual Camera or equivalent camera input
- **Storage**: A few hundred MB for the app and model files downloaded on first launch

## Community

- [Report a Bug](https://github.com/fufufukakaka/pokemon_champions_battle_logger/issues/new?template=bug_report.yml)
- [Request a Feature](https://github.com/fufufukakaka/pokemon_champions_battle_logger/issues/new?template=feature_request.yml)
- [Discord](https://discord.gg/37ApwRvUrW)
- [X (Twitter)](https://x.com/pokechampbatlog)

## Support Development

This is a personal project, and continued improvement takes time, testing, and maintenance. If the app helps you, you can support development on Buy Me a Coffee.

<p align="center">
  <a href="https://www.buymeacoffee.com/fufufukakaka" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" height="60" width="217"></a>
</p>

## License

This software is released under a proprietary **All Rights Reserved** license.

You are permitted to download the Software from the official distribution channel (GitHub Releases) and use it for **personal, non-commercial purposes**. **Redistribution, modification, reverse engineering, and commercial use are prohibited.**

See [LICENSE](LICENSE) for full terms.

---

<p align="center">Made with love for Pokemon Trainers</p>
