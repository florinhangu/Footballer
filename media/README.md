# Screenshot provenance

## Standalone editor 1.2.26 — British English and application icon

The six UI captures in `media/editor-1.2.26/` come from
`docs/screenshots/editor-english-2026-11-01/` in the game source at
[`2f93ecd04be196ffd289210279fe29b0a7306503`](https://github.com/florinhangu/no9dayone/commit/2f93ecd04be196ffd289210279fe29b0a7306503).
They show the exported standalone No9Editor 1.2.26 pack, with its own database and
the Dummy audio driver, without game autoloads other than the independent shared
localisation service. They were visually inspected and copied without retouching.

`english-federations.png`, `english-clubs.png` and `english-rules.png` show the
translated forms, English-name search and readable regulations.
`federation-jersey-models.png`, `federation-shorts-models.png` and
`federation-kit-back.png` show garment-only, club-coloured model grids and selected
printing fonts. The application remains separate from the game.

`no9editor-icon.png` is the original No9 football-and-pencil vector artwork,
rasterised from `assets/editor/no9editor-icon.svg`; it is an application asset,
rather than a screenshot. The Windows executable embeds multiple icon sizes.
These images do not establish mobile performance or completion of the game's
separate dialogue localisation review.

## Standalone editor 1.2.25 captures

The four images in `media/editor-1.2.25/` are unedited copies of `docs/screenshots/editor-kit-gallery-colors-2026-11-01/` at source commit [`fa41dedaf2bd`](https://github.com/florinhangu/no9dayone/commit/fa41dedaf2bde9fd19ec510f15496ab751a9fe99). They were captured from the separate exported No9Editor 1.2.25 application with audio driver Dummy, then visually inspected. The shirt, shorts and socks popups show the selected team kit colors; the back preview shows independently chosen name and number fonts. They do not show an editor embedded in the game. The earlier media collections below retain their original versions and source snapshots.


## New captures — 1 November 2026

The six files under `media/updates-2026-11-01/` are unedited copies of actual Godot captures. The friendly uses the game's shared match renderer with a controlled camera and isolated season-five state. The editor images were captured from the **exported standalone No9Editor 1.2.23 pack**, with its own database and without the game's autoloads. They show separate applications and are labelled accordingly; no image was generated with AI.

| Public file | Original game repository path | Context |
| --- | --- | --- |
| season-5-home.png | docs/screenshots/season-kits-2026-11-01/season-5-home.png | Chelsea's three-piece kit; saved 2D shirts shown in the corners |
| season-5-away.png | docs/screenshots/season-kits-2026-11-01/season-5-away.png | Pacífico FC's independently colored kit in the same friendly |
| season-5-friendly.png | docs/screenshots/season-kits-2026-11-01/season-5-friendly.png | Actual 22-player friendly renderer, season-five team kits |
| club-kit-form.png | docs/screenshots/editor-kits-2026-11-01/club-kit-form.png | Standalone editor's club garment models and three-color controls |
| federation-kit-preview.png | docs/screenshots/editor-kits-2026-11-01/federation-kit-preview.png | Exported editor's front SS/LS kit preview for Romania |
| federation-kit-back.png | docs/screenshots/editor-kits-2026-11-01/federation-kit-back.png | Same exported preview from behind |

Source snapshot: [`01d3dc3da5c6`](https://github.com/florinhangu/no9dayone/commit/01d3dc3da5c6dfc63580d97309b0c22c12b41376). Capture tools: `tools/capture_season_team_kits.gd` and `tools/capture_editor_kit_schedule.gd`. The captures were visually inspected. They demonstrate desktop rendering and kit selection; they do not establish mobile performance, a public APK release or a full unassisted match playthrough.

The historical archived images were copied from the No9: Day One development snapshot b52aeca28f3a7ac83cf2ed1a32a8393217d53d18. A second collection below contains newly verified media present at source commit 1b6d67459ae5bcaf5bb0f587e9131839c0a642cb. The historical collection below retains its original provenance. Newer game and standalone-editor captures are identified separately by date and application.

| Published file | Original development path | Last commit date (UTC) | Context |
| --- | --- | --- | --- |
| media/career.png | docs/screenshots/career.png | 2026-10-04 | Career home / trial |
| media/match-2d.png | docs/screenshots/match.png | 2026-10-04 | Existing 2D match |
| media/training-campus.png | docs/model25d/training-premium/overview.png | 2026-10-11 | Premium test-campus overview; archived, not shown in README |
| media/player-run.png | docs/model25d/runtime/match-actions/run.png | 2026-10-09 | Native player test; archived, not shown in README |
| media/player-keeper.png | docs/model25d/runtime/match-actions/keeper-tracking.png | 2026-10-09 | Native player test; archived, not shown in README |
| media/base-single.png | docs/model25d/training-single/overview-mobile.png | 2026-10-09 | Training-base test overview; archived, not shown in README |
| media/base-classic.png | docs/model25d/training-base/overview-mobile.png | 2026-10-09 | Training-base test overview; archived, not shown in README |
| media/base-academy.png | docs/model25d/training-academy/overview-mobile.png | 2026-10-09 | Training-base test overview; archived, not shown in README |
| media/base-performance.png | docs/model25d/training-performance/overview-mobile.png | 2026-10-09 | Training-base test overview; archived, not shown in README |
| media/training-3d.png | docs/model25d/runtime/training-360.png | 2026-10-08 | Earlier free-training test capture; retained, not in current gallery |
| media/customization.png | docs/model25d/runtime/customization-face.png | 2026-10-08 | Earlier appearance test; retained, not in current gallery |
| media/training-result.png | docs/model25d/runtime/catalog/result-360.png | 2026-10-08 | Earlier test result; retained, not in current gallery |

A last-commit date establishes when an image entered Git, not the actual capture time. The remaining README screenshots show the existing career and 2D match, with their original dates.

This statement described the earlier 13 October review only. The 28 October review found newer committed official 3D career screenshots, Solv3 action recordings and No9Editor captures dated 25–27 October. These assets were copied from the No9 repository, not created as mockups.

The archive includes separate original, classic, academy, performance and premium bases. Their images are excluded from the README because their capture process does not establish a run of the complete game.

The screenshots show Romanian UI. Keyboard or action buttons visible in archived test images are developer testing tools.

Source paths are provenance records, not public image URLs. Archived copies remain in this repository. The isolated sprint/energy HUD image from 13 October has been removed from the public media collection; it is not evidence of the complete game's appearance. No promotional image was generated with AI.

Logos have their own [source and terms](branding/README.md).

## New source-backed media · 25–27 October 2026

All files in `media/updates-2026-10-27/` are **byte-identical Git blobs** from `florinhangu/no9dayone` at source commit [`1b6d67459ae5`](https://github.com/florinhangu/no9dayone/commit/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb). They were not AI-generated or redrawn. Screenshots from controlled regression runs demonstrate the actual Godot presentation, **not gameplay recorded on Android/iOS**. The official result UI was captured in a short scenario ending under test control; its 0–0 statistics are not the result of the separate full-match regression. Solv3 player/goalkeeper and GIF scenes are showcase/test scenes and are labelled accordingly.

| Footballer image / animation | Original game repository path | Context |
| :-- | :-- | :-- |
| [official-match-720p.jpg](updates-2026-10-27/official-match-720p.jpg) | [docs/screenshots/game-portrait-reserves/official-match-720p.jpg](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/game-portrait-reserves/official-match-720p.jpg) | Official career 3D, 720×1280 portrait, controlled UI capture |
| [official-result-720p.jpg](updates-2026-10-27/official-result-720p.jpg) | [docs/screenshots/game-portrait-reserves/official-result-720p.jpg](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/game-portrait-reserves/official-result-720p.jpg) | Official career result UI, controlled short scenario |
| [solv3-actions.jpg](updates-2026-10-27/solv3-actions.jpg) | [docs/screenshots/solv3/authored-actions-overview.jpg](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/solv3/authored-actions-overview.jpg) | Godot Solv3 animation and referee showcase |
| [solv3-player.png](updates-2026-10-27/solv3-player.png) | [docs/screenshots/solv3/field-720p.png](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/solv3/field-720p.png) | Solv3 player scene |
| [solv3-goalkeeper.png](updates-2026-10-27/solv3-goalkeeper.png) | [docs/screenshots/solv3/keeper-720p.png](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/solv3/keeper-720p.png) | Solv3 goalkeeper model with gloves |
| [solv3-mocap.jpg](updates-2026-10-27/solv3-mocap.jpg) | [docs/screenshots/solv3/mocap-2026-10-26/overview.jpg](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/solv3/mocap-2026-10-26/overview.jpg) | Accepted mocap source action comparisons |
| [editor-1.2.17.png](updates-2026-10-27/editor-1.2.17.png) | [docs/screenshots/editor-commercial-1.2.17/editor-commercial.png](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/editor-commercial-1.2.17/editor-commercial.png) | No9Editor 1.2.17 desktop interface |
| [editor-kit-preview.png](updates-2026-10-27/editor-kit-preview.png) | [docs/screenshots/editor-commercial-1.2.17/shirt-front.png](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/editor-commercial-1.2.17/shirt-front.png) | 3D kit branding preview inside editor |
| [data-packages.png](updates-2026-10-27/data-packages.png) | [docs/screenshots/database-packages-2026-10-25/editor-packages-720p.png](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/database-packages-2026-10-25/editor-packages-720p.png) | In-game data packages UI |
| [standing-tackle.gif](updates-2026-10-27/standing-tackle.gif) | [docs/screenshots/solv3/standing_tackle_right.gif](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/solv3/standing_tackle_right.gif) | Published Solv3 tackle playback |
| [referee-card.gif](updates-2026-10-27/referee-card.gif) | [docs/screenshots/solv3/referee_card.gif](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/screenshots/solv3/referee_card.gif) | Published Solv3 referee-card playback |

The visible game UI is Romanian. The public README remains an English-language presentation. Media references are descriptive rather than a certification of the assets' final aesthetic quality or mobile performance.
