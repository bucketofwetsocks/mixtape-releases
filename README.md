# Skittle

**A randomizer for Super Mario World romhacks.** Roll any hack from the SMWDB / SMW Central catalog and get dropped straight into a random playable level — no overworld navigation needed.

## Download

Head to the **[Releases](../../releases)** page and grab the latest `Skittle-vX.Y.Z-win64-portable.zip`.

Unzip and read `FIRST-RUN.txt` for setup. The whole folder is self-contained — copy/move it anywhere.

## Requirements

- **Windows x64**
- **[RetroArch](https://www.retroarch.com/?page=platforms)** with an SNES core (`snes9x_libretro` recommended; `bsnes_mercury` also works). Install RetroArch, then use its Online Updater → Core Downloader to grab a core.
- **A clean Super Mario World base ROM** — your own copy. We can't legally distribute SMW; you provide your own `.smc`.

Once you've installed RetroArch + a core and have your SMW.smc, launch `skittle.exe` and point the Settings page at all three (RetroArch path, core path, SMW base ROM). Then refresh the catalog and roll.

## What it does

- Picks a random hack from a local catalog of SMWDB + SMW Central entries (filterable by category, difficulty, year, HoF status).
- Patches the hack on the fly with a custom **No-Overworld** asar patch that skips the title/overworld and drops you straight into a chosen playable level.
- Plays it in your RetroArch.

## Known limits

- Some hacks (especially older ones SMW Central / SMWDB tag as `[BAD-emu]`) may not behave correctly under emulation. We aim to support most, but not every hack will work.
- You're playing a single level out of the larger hack's context — story, mechanics, or hints introduced in other levels will be missed by design.

Be kind to the original hack authors. They put real work in.

## Project

The source code lives in a separate private repository. This repo exists purely to host the public release downloads.
