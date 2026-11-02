# Public builds

[Open Footballer Releases](https://github.com/florinhangu/Footballer/releases).

## No9Editor 1.2.26 — 2 November 2026

**[Download the standalone Windows editor](https://github.com/florinhangu/Footballer/releases/download/no9editor-v1.2.26/No9Editor.exe)** · **[Release notes and SHA-256](https://github.com/florinhangu/Footballer/releases/tag/no9editor-v1.2.26)**

This is a separate single-file editor for Windows x86-64, with British English as
the default and a selectable Romanian catalogue. It includes the independent
three-piece kit editor, club-coloured 72×72 model grids, custom printing fonts,
stadium editing and portable projects/data packs. Godot is not required to run it.
See the [editor guide](EDITOR.md) and [verification notes](VERIFICATION.md).

File: `No9Editor.exe` — **560,848,640 bytes**.

SHA-256: `94dbc37880e91e6b372ff70a892832e30fc7815f5c7c0d56d2a6d154b99f059c`.

The public release includes the executable and `SHA256SUMS.txt`. This release does
not include an Android game APK.

## Game build target

Android APK, portrait interface, ARM32 and ARM64. No verified iOS export preset or release was found.

The current game source reports development version **0.A1.19** (27 October 2026). The older, conflicting export/version metadata documented on 12 October is historical and must be rechecked against the final source and Android build before publishing. Neither the version number nor the screenshots establishes a tested public APK.

## What each release should tell a player

- Exact version and source snapshot.
- Included career, training and 3D test modes.
- APK filename and checksum.
- Android devices and OS versions actually tested.
- Known issues, especially loading, animation and 3D performance.
- Whether existing saves remain compatible.

## Installing a future Android build

Download the APK attached to a published release, allow installation from the browser or file manager when Android requests it, and install. Follow that release's instructions for updates and saves.

There is currently no APK link to substitute for a missing release. The source export path is a development setting, not a public download.

## Suggested release-note outline

### Added / improved
Describe the changes a player can see.

### Verified
Name the actual devices and modes tested.

### Known issues
State reproducible limitations.

### Saves
Explain compatibility and any required backup.

### Download
Attach the tested APK and checksum.
