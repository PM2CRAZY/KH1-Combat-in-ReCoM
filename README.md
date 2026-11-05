# KH1 Combat in Re:Chain of Memories (release)

A mod that brings Kingdom Hearts Final Mix's combat to Sora in Kingdom Hearts Re:Chain of Memories
(PC, Steam, KH 1.5+2.5), built into Re:CoM's own systems.

This repository holds **only the release build** (version in `VERSION`), updated when the
author says a version is ready. Development, the source and the latest test builds are in
[PM2CRAZY/KH1-in-ReCom](https://github.com/PM2CRAZY/KH1-in-ReCom) (branch `testing`).

## Requirements

- **KINGDOM HEARTS HD 1.5+2.5 ReMIX on Steam (PC)**, with **Kingdom Hearts Final Mix** and
  **Re:Chain of Memories** both installed (the same collection folder). The mod builds its KH1
  files from your own KH1 and Re:CoM files; no game files are shipped.
- **OpenKH Mods Manager** set up for the PC version, with **Panacea** installed (the Mods
  Manager's setup wizard does both).

## Install (OpenKH, from GitHub)

1. Open the OpenKH Mods Manager and select **Kingdom Hearts Re:Chain of Memories** in its game list
   (the mod is installed for the game selected at that moment).
2. Mods → **Install a new mod** → type `PM2CRAZY/KH1-Combat-in-ReCoM` → Install. (For the latest
   test builds instead, install `PM2CRAZY/KH1-in-ReCom/testing`; don't enable both at once.)
3. Tick the mod and press **Build** (or **Build and Run**).
4. Start Re:CoM. **On the first start the mod builds the KH1 files** from your games: the title
   screen shows "KH1 in Re:CoM: building files from your games... N %" and the step it is on, and
   waits. When it says "done", the title goes on by itself. No second Build, no restart.
5. Next to the game exe you'll find `kh1-recom.log` (what the mod did), `kh1-recom-build.log` (the
   build's details) and `kh1-recom.ini` (settings, also in the camp menu).

The built files stay in the mod's folder (`generated/`) and are copied into OpenKH's mod folder
at each start (a Build removes that copy; the next start puts it back). They are rebuilt only when
an update changes how they're made, or when the game itself is updated.

If KH1 Final Mix is not installed, the title says "KH1 FM not found: playing without KH1 files" and
the game goes on without them.

**Updating:** in the Mods Manager, check for updates and update the mod, then Build.
