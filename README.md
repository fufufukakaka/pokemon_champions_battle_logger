# Pokemon Champions Battle Logger

<p align="center">
  <img src="https://img.shields.io/github/v/release/fufufukakaka/pokemon_champions_battle_logger?style=flat-square&color=FF3B30" alt="Release">
  <img src="https://img.shields.io/github/downloads/fufufukakaka/pokemon_champions_battle_logger/total?style=flat-square&color=00B4DC" alt="Downloads">
  <img src="https://img.shields.io/badge/platforms-Windows%20%7C%20macOS%20%7C%20Linux-32D74B?style=flat-square" alt="Platforms">
  <img src="https://img.shields.io/badge/license-MIT-555?style=flat-square" alt="License">
</p>

<p align="center">
  <strong>Dominate Your Battle Data.</strong><br>
  Pokemon Champions Battle Logger automatically records and analyzes your battles from video.
</p>

---

## Features

- **Auto Battle Detection** - Drop a YouTube URL or local video file, and AI automatically detects battles, recognizes Pokemon, reads moves, and determines win/loss
- **Deep Analytics** - Win rate trends, team selection stats, knockout statistics, all visualized in real-time dashboards
- **8 Languages** - Japanese, English, Traditional Chinese, Simplified Chinese, Korean, French, Spanish, Italian, German
- **100% Local** - Your data stays on your machine. No cloud, no accounts, no tracking
- **Free & Open Source**

## Download

> **Latest Release**: [Download here](https://github.com/fufufukakaka/pokemon_champions_battle_logger/releases/latest)

| Platform | File |
|----------|------|
| Windows (x64) | `poke-champions-logger-windows-x64.zip` |
| macOS (Apple Silicon) | `poke-champions-logger-macos-arm64.tar.gz` |
| macOS (Intel) | `poke-champions-logger-macos-x64.tar.gz` |
| Linux (x64) | `poke-champions-logger-linux-x64.tar.gz` |

### Quick Start

1. Download the archive for your platform from [Releases](https://github.com/fufufukakaka/pokemon_champions_battle_logger/releases/latest)
2. Extract the archive
3. Run `poke_champions_logger` (or `poke_champions_logger.exe` on Windows)
4. The app opens in your browser at `http://127.0.0.1:8000`
5. Follow the initial setup wizard (choose language, enter trainer name)

### macOS Users

macOS may show a security warning for unsigned apps. To bypass:

```bash
xattr -cr /path/to/poke_champions_logger
```

Or right-click the app and select "Open" instead of double-clicking.

## Screenshots

<!-- TODO: Add screenshots -->

*Coming soon*

## Requirements

- **Video input**: 1920x1080 (1080p) video
- **Format**: Single battles in Pokemon Champions
- **Storage**: ~500MB for the app + model files downloaded on first launch

## Community

- [Report a Bug](https://github.com/fufufukakaka/pokemon_champions_battle_logger/issues/new?template=bug_report.yml)
- [Request a Feature](https://github.com/fufufukakaka/pokemon_champions_battle_logger/issues/new?template=feature_request.yml)
<!-- - [Discord](https://discord.gg/XXXXX) -->

## For Developers

If you want to run from source or contribute:

```bash
# Clone the development repository
git clone https://github.com/fufufukakaka/poke_battle_logger_2.git
cd poke_battle_logger_2

# Install dependencies
uv sync --all-extras

# Run development server
make dev
```

See the [development repository](https://github.com/fufufukakaka/poke_battle_logger_2) for more details.

## License

MIT License. See [LICENSE](LICENSE) for details.

---

<p align="center">Made with love for Pokemon Trainers</p>
