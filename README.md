# MixTape

A Windows desktop app for building and playing curated mixes of Super Mario World ROM hacks. Point it at your clean SMW base ROM, pick some hacks and levels, and MixTape patches them on the fly, launches your emulator, and moves you through the run without any overworld or menus in between.

## Main features

### Builder
- Assemble a run from **KaizOFF** or local ROM folders — mix sources freely inside a single run.
- **Scripted runs** — pick the exact hacks and levels yourself.
- **Seeded runs** — pick the hacks and (optionally) curated level pools; a seeded RNG deterministically rolls a set. Same seed always plays the same levels.
- **Per-run description + author** so credits and context ride along with the mix.

### Runner
- Paste a base64 share code or drop in a `.mixtape` file — MixTape resolves the hacks, patches them, and drops you into the run.
- Patches and hashes cache after the first play, so re-runs are instant.

### Sharing
- **Share code** — a base64 string encoding the entire run (name, author, description, hacks, levels, graph, goals). Paste it into anyone else's copy of MixTape.
- **Discord Share** — one click copies a formatted message (`**Mix name** by Author — Description` + fenced code block) to your clipboard.
- **Portable mix** (`.mixtape` file) — a zip carrying the BPS patch for every hack, so the recipient can play the mix even without the source hacks locally.

### Emulator + hardware support
- **RetroArch** with the snes9x core — auto-launched with the current ROM.
- **FXPak Pro** via SNI — play on real hardware, with automatic reconnect on cart hiccups and retries on flaky USB frames.

## Download

Portable zips ship as `MixTape-v<version>-win64-portable.zip` from
[github.com/bucketofwetsocks/mixtape-releases](https://github.com/bucketofwetsocks/mixtape-releases).
Unzip, run `mixtape.exe`, point Settings at your clean SMW base ROM,
refresh the catalog, and go.
