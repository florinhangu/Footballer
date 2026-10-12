# Verification notes

Reviewed: 12 October 2026. Source baseline: b52aeca28f3a7ac83cf2ed1a32a8393217d53d18.

This presentation was prepared through a read-only source/history review. Godot was not run, an APK was not built, and the desktop tests below were not rerun. Reported results come from existing project documentation.

## Evidence and scope

| Existing source document | What it records |
| --- | --- |
| docs/model25d/player-showcase/demo-match.md | 10–11 October desktop simulations, native animation checks and explicit historical failures |
| docs/model25d/basic-stadium.md | Shared-authority integration, referee/substitution/loading checks and desktop rendering measurements |
| docs/model25d/official-3d-match-adapter.md | Authoritative fixture interface, presentation responsibilities and remaining career integration work |
| project.godot / export_presets.cfg | Compatibility renderer, portrait Android target and conflicting application/export version strings |

These paths identify documents in the development source; they are not public download links.

The current source uses Humanizer-based actors. Historical Lunin/exported-male GLBs, their old character controller and the old model3d/football_motion smoke scripts are absent from the reviewed tree. Their old screenshots and test results do not establish current model quality.

## Reported results

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

No source recovery, revert, merge or gameplay edit was performed for this page.

## Public presentation boundaries

The working career features are presented as available. Native 3D test pages, players, facilities and stadium demonstrations are presented as future development. Match input is exclusively tap and swipe; physical controls and action buttons belong only to developer test pages.
