# No9Editor 1.2.26

No9Editor is a **separate standalone application for 64-bit Windows**. It creates
projects and data packs for No9: Day One. The single executable includes its own
runtime, reference database and assets; installing or opening Godot is unnecessary.

Its custom football-and-pencil icon is embedded in the executable, with multiple
sizes for Windows desktop shortcuts and the taskbar.

[Download No9Editor.exe](https://github.com/florinhangu/Footballer/releases/download/no9editor-v1.2.26/No9Editor.exe)
or open the [release page](https://github.com/florinhangu/Footballer/releases/tag/no9editor-v1.2.26)
for the checksum and verification details. The file is approximately 535 MiB.

## British English and other languages

British English is the default. Use **Language** in the top toolbar to select
**English (UK)** or **Română**. Separate catalogue files keep the languages
independent, and the application remembers your choice. Further languages can
be included in future builds without mixing their text with existing catalogues.

Conventional English team names include **Real Madrid**, **Steaua Bucharest**,
**Bayern Munich** and **Red Star Belgrade**. Search accepts original or English
display names. Saving an untouched translated name retains the original stored
value; explicitly authored text remains the author's choice. IDs are unchanged.

## What you can edit

| Category | Available changes |
| --- | --- |
| Federations | Name, national-team rating, identity colours, stadium and kits |
| Leagues | Name and membership for new careers |
| Competitions | Name |
| Clubs | Name, short name, ratings, colours, stadium, kits and branding |
| Stadiums | Name, capacity, stands, corners, roofs, equipment and environment |
| Regulations | Readable reference pages |

The kit model button opens a grid of unnamed thumbnails up to **72×72**.
Shirt, shorts and socks each show their own playable designs, ordered numerically;
UV guides are excluded. Thumbnails use the current garment's kit colours. Choose
a tile to close the grid and retain that selection. Each garment's model and
colours remain independent. The 3D preview supports both sleeve lengths and a
front/back view. Name and number have independent font choices, including imported
TTF/OTF fonts embedded in exported projects and packs.

## Save, export and use

1. Use **Save changes** to keep the editor's working project.
2. Use **Save project as…** for a portable `.no9project` that another copy of the
   editor can reopen.
3. Choose **Export pack…**, select the changes to share, and create a `.no9pack`.
4. Import the pack through the game's data-pack interface, activate it, set its
   priority and confirm the selection.

Imported packs have their own local copies. Changes to different fields combine;
conflicting values require an explicit priority choice. Existing projects and
packs retain their identifiers. The editor does not rewrite the game's bundled
database or require the game to be installed beside it.

New careers can use activated changes from the start. Existing careers stage
presentation changes for the next season boundary. League membership and the
three initial ratings apply only to new careers.

An authored kit applies for **one normal kit edition in each career**, waiting
for the team's scheduled change: annually in L1 and every two seasons in L2/L3
and for national teams. Normal random generation resumes afterwards. Another
actual kit edit can provide a new authored edition; an unrelated name or stadium
edit does not reactivate it.

## Verified scope

The release was tested on Windows using the exported standalone pack, isolated
test data and the Dummy audio driver. **199 focused checks passed**, alongside
captures of all six editor categories, language switching and kit model galleries.
The installed file and uploaded asset have the same SHA-256 as the tested export.
See [verification notes](VERIFICATION.md#standalone-editor-126-british-english--2-november-2026).

This is a Windows editor release. Game dialogue localisation remains under review;
no public Android game build is included in this release.
