# Verification notes

Reviewed: 13 October 2026. Current source baseline: f7e6b4bcc785e967677dd2d4d3a15ebc0e5fc0d5. The earlier presentation review used b52aeca28f3a7ac83cf2ed1a32a8393217d53d18.

The original presentation used a read-only source/history review. On 13 October, the sprint implementation was validated in focused desktop runs with Godot 4.7.2 and isolated test storage. The HUD was rendered and visually inspected in an isolated test project, without running the complete game. No APK was built or tested on an Android device. Earlier simulation/performance results remain historical documentation, separate from the new focused checks.

## Sprint update — executed desktop checks

| Test | Checks | Failures |
| --- | ---: | ---: |
| player_sprint_regression | 39 | 0 |
| player_sprint_input_regression | 9 | 0 |
| football_gestures_regression | 13 | 0 |
| match_integrity_regression | 129 | 0 |
| Total | 190 | 0 |

The checks cover gesture recognition, immediate first-tap movement, possession-only sprint, off-ball AI, opponent-tap tackling, canceled/multiple pointers, resource exhaustion/recovery, speed/acceleration/stamina effects, pause and stationary-possession freeze, real-second rates at 1.75× and 2.75× tempo, exact HUD values, narrow-screen layout and the sprint gear in the 3D history buffer. These checks do not constitute a full native 3D scene run or Android acceptance test.

The source audit inventoried all 10,739 tracked files in the pre-sprint baseline, inspected 485 GDScript files and checked external references in 152 text scenes. Binary assets were inventoried rather than individually rendered. The audit identified local sky/water/ground resources excluded from Git; full native 3D verification requires the complete local asset installation.

The HUD was rendered in an isolated desktop test harness. That capture is excluded from the public presentation because it does not show the complete game's actual layout. The sprint update has not been verified in a played match in the complete game.

## Evidence and scope

| Existing source document | What it records |
| --- | --- |
| docs/model25d/player-showcase/demo-match.md | 10–11 October desktop simulations, native animation checks and explicit historical failures |
| docs/model25d/basic-stadium.md | Shared-authority integration, referee/substitution/loading checks and desktop rendering measurements |
| docs/model25d/official-3d-match-adapter.md | Authoritative fixture interface, presentation responsibilities and remaining career integration work |
| project.godot / export_presets.cfg | Compatibility renderer, portrait Android target and conflicting application/export version strings |

These paths identify documents in the development source; they are not public download links.

The current source uses Humanizer-based actors. Historical Lunin/exported-male GLBs, their old character controller and the old model3d/football_motion smoke scripts are absent from the reviewed tree. Their old screenshots and test results do not establish current model quality.

## Earlier reported results

- 10 October autonomous demo: 90 seconds, 31 passes, 15 shots, eight ground goalkeeper distributions, score 1–1.
- 11 October official-AI demo: 90 seconds, 11 passes, seven crosses, four shots, 14 headers, 12 received passes, seven goalkeeper distributions, score 1–0.
- Native library comparison: 7,685 checks, zero failures.
- Focused shared-authority/presentation integration: 684 checks, zero failures.
- Wider tactical suite: 25 failures in 58 checks.
- Wider world-state suite: two failures in 58 checks.
- Earlier documentation also records goal-kick suite failures, 192/288, against its corresponding baseline.

Different test suites and snapshots cannot be added into one universal pass rate. Controlled scenarios deliberately exercise rare actions; one autonomous match is not statistical evidence of balance.

## Performance limits

A documented Godot 4.7.2 Compatibility run on GTX 1050, 696 × 900, 22 players plus native referee and 1.75× tempo measured 33.553 ms median and 65.757 ms p95. A later run concurrent with GPU loading measured 49.176 ms median and 68.904 ms p95. Loading documentation reports a longest frame around 883 ms.

These are source-reported measurements, not fresh benchmarks. They do not prove Android frame rate or a continuously smooth loading animation.

## Smallest next verification plan

1. Keep the current source baseline fixed. Verify walk → run → idle transitions and soles on the pitch, including the live actor and baked showcase.
2. Run the existing gait-floor, animation-form, Humanizer geometry/render and jersey-print checks. Confirm left/right limbs, skin bindings, body/clothes masking and both boots visually.
3. Run the authoritative-match and loading-render checks. Inspect walk-in, line-up, half-time, second-half entry, substitution and both cameras.
4. Test one Android device with the actual release APK; record device, renderer, frame times, loading and save compatibility.
5. Reconcile version metadata and publish only the APK that passed those checks.

The transition change introduced by commit 8fada4279e660b2c8dd5dfac5a7dc9f0994c3418 remains in the reviewed player controller after the camera restoration. This is a candidate for focused verification, not a confirmed runtime defect.

The old boot-replacement report preserved length but increased width by about 6.1% and height by about 10.5%; the corresponding old asset is no longer current. Restoring it globally would reintroduce obsolete rig assumptions.

The sprint implementation is in the private game source. This public repository contains the presentation, documentation and screenshots.

## Public presentation boundaries

The working career features are presented as available. Native 3D test pages, players, facilities and stadium demonstrations are presented as future development. Match input is exclusively tap and swipe, with rapid double-tap sprint only in possession. Off-ball positioning stays under AI and opponent taps request a tackle; physical controls and action buttons belong only to developer test pages.
