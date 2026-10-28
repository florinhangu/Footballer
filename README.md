<div align="center">

# No9: Day One

### Your first trial. Your first contract. Your story on the pitch.

**A football career begins with a chance. What you do with it is up to you.**

Offline player career · 2D and official 3D matches · Touch-first football · Living competitions

<img src="media/snapshots/Screenshot%202026-10-13%20190839.png" width="35%" alt="No9 live 2D football match"> <img src="media/updates-2026-10-27/official-match-720p.jpg" width="35%" alt="Official native 3D career match from the real Godot game">

**[Explore the game](#the-footballer-is-you) · [See the screenshots](#official-game-snapshots) · [Public releases](https://github.com/florinhangu/Footballer/releases)**

</div>

## Latest game milestone — 27 October 2026

**No9: Day One / No9 GameCore · game 0.A1.19 · Godot 4.7.2**

The career now supports **official 3D matches**, rather than limiting 3D to a separate demonstration. In **Configurator → Afișare meci oficial**, choose **3D** (the default remains **2D**). The fixture uses its actual teams, stadium and career footballer. The 2D and 3D presentations share the same **AuthorityEngine** match rules, result calculation, match statistics and career persistence. Youth trials still use the existing 2D path.

The updated match view fills the available **9:16 portrait** width with an overlaid score, match information and sprint/energy bars. Competitive official fixtures show **up to nine substitutes per team**; friendlies retain up to fifteen. The 3D view offers TV and ball cameras and speeds of **0.5×, 1×, 1.25× and 1.5×**. Results, minutes, player ratings and statistics return to the career after **Continuă**.

<div align="center">
  <img src="media/updates-2026-10-27/official-match-720p.jpg" width="30%" alt="Actual official career 3D match running in the No9 Godot scene">
  <img src="media/updates-2026-10-27/official-result-720p.jpg" width="30%" alt="Actual match statistics and Continue screen in the Godot career scene">
  <img src="media/snapshots/Screenshot%202026-10-13%20190839.png" width="30%" alt="Established 2D career match">
  <br><sub>Left and center: official 3D career UI captured in desktop Godot; right: original 2D career match. The 3D screenshots are controlled short scenarios, not evidence of a full Android playthrough.</sub>
</div>

The development reports record **439 focused checks with no failures** for the portrait HUD, substitutes, camera continuity and related 2D/3D paths. Separate official-career tests exercised two halves and saving/reloading the result. These are **reported desktop regression tests**, not Android/iOS acceptance, stable mobile-FPS certification or a published APK. See the [portrait and bench audit](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/audits/game-portrait-reserves-2026-10-27.md) and the [career integration report](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/audits/career-3d-integration-2026-10-27.md).

### New Solv3 footballer, goalkeeper and motion captures

The current native character pipeline uses **Solv3** and one shared **130-clip animation library**, including four approved additional mocap sequences and ten new authored actions. Those actions include standing tackles, a left-foot penalty and referee signals. The goalkeeper uses a long-sleeved top and separate gloves. The football, goalkeeper and referee are shown here from **actual project scenes and baked animations**, not from unrelated concept renders.

<div align="center">
  <img src="media/updates-2026-10-27/solv3-player.png" width="28%" alt="Solv3 in-game footballer rig and kit">
  <img src="media/updates-2026-10-27/solv3-goalkeeper.png" width="28%" alt="Solv3 goalkeeper wearing gloves and long sleeves">
  <img src="media/updates-2026-10-27/solv3-mocap.jpg" width="40%" alt="Approved mocap action poses from the native Solv3 pipeline">
</div>

<p align="center"><img src="media/updates-2026-10-27/solv3-actions.jpg" width="92%" alt="Godot-baked authored football and referee actions"></p>

<details>
<summary><strong>Watch real animated previews — tackle and referee card</strong></summary>
<p align="center"><img src="media/updates-2026-10-27/standing-tackle.gif" width="45%" alt="Godot baked standing-tackle action"><img src="media/updates-2026-10-27/referee-card.gif" width="45%" alt="Godot baked referee card signal"></p>
</details>

### New desktop editor and data-package views

**No9Editor 1.2.17** introduced editable branding for kit sponsors, advertisements and manufacturer logos, as well as more complete portable data packages. The subsequent **1.2.18** desktop installation was checked alongside the optimized match environment. Saved editor stadium configurations can also be exported and loaded into the actual 3D match. The following images show the editor and kit preview, plus the game's in-app package screen; they are **different interfaces**, not three views of the same screen.

<div align="center">
  <img src="media/updates-2026-10-27/editor-1.2.17.png" width="49%" alt="No9Editor desktop application, release 1.2.17">
  <img src="media/updates-2026-10-27/editor-kit-preview.png" width="49%" alt="Actual player shirt branding preview from No9Editor">
  <br><img src="media/updates-2026-10-27/data-packages.png" width="30%" alt="Native in-game package management screen">
</div>

See the [editor documentation](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/no9editor.md), [Solv3 action audit](https://github.com/florinhangu/no9dayone/blob/1b6d67459ae5bcaf5bb0f587e9131839c0a642cb/docs/audits/solv3-actions-2026-10-27.md), and [media provenance](media/README.md).

## The footballer is you

**No9: Day One** is a football player-career game built for mobile. You are not the club manager watching from the sidelines. You create a footballer, earn your first opportunity at a trial, sign a contract, train for your place in the squad and live with the consequences of every match and every season.

Start young. Find a team willing to give you a chance. Grow your abilities, earn minutes, make the most of the ball and decide where your career will go. Beyond your own pitch, leagues keep moving: tables change, clubs earn promotion or face relegation, cup campaigns continue and international opportunities emerge.

The game is designed around **offline progression and local saves**. Official career matches can now use **2D (default) or native 3D**; youth trials remain on the 2D route. Dedicated native 3D training, character and stadium development scenes also remain available. This implementation has been tested on desktop; mobile performance and release readiness are still to be verified.

## The experience today

| Your journey | On the pitch | The football world |
| :-- | :-- | :-- |
| Create your player and start at youth trials | Live 2D matches with football AI and match officials | Domestic leagues, cups and changing tables |
| Compete for contracts and a starting place | Tap, double tap and swipe controls | Regional divisions, play-offs and promotion battles |
| Develop attributes through training and recovery | Passing, crossing, shooting, challenges and set pieces | International club and national-team competitions |
| Follow energy, form, club life and history | Sprint and energy reserves tied to player abilities | Thousands of clubs across six geographic regions |
| Track your club, fixtures, career and trophies | Optional official 3D career matches, plus native practice scenes | A world that continues through successive seasons |

### From the first trial to the next season

Your career begins by defining a player: position, preferred foot, country and footballing identity. Youth trials provide the first test. Contract offers open the door to a club, where every week brings another training decision, upcoming fixture, possible injury or new challenge.

Your profile keeps track of skills, contracts, official match history and trophies. Weekly scheduling connects training, recovery, matches and club responsibilities. The **60-week season structure** keeps domestic and international football moving in the same career.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20184846.png" width="27%" alt="Player profile and football abilities">
<img src="media/snapshots/Screenshot%202026-10-13%20184932.png" width="27%" alt="Career calendar and football fixtures">
<img src="media/snapshots/Screenshot%202026-10-13%20184915.png" width="27%" alt="Team tactics and formation">
</div>

## Tap. Swipe. Play.

On the career pitch, matches unfold in real time. Team-mates and opponents use AI to make runs, support each other, defend and respond to game situations. You influence the game through the footballer you control.

| Gesture | Action |
| :-- | :-- |
| **Tap an open area** | Move or dribble there while in possession |
| **Quick double tap** | Sprint with the ball toward the selected point |
| **Swipe toward a team-mate** | Play a pass |
| **Long swipe toward a team-mate** | Deliver a longer / aerial ball |
| **Swipe toward goal** | Attempt a shot |
| **Tap an opponent in a duel** | Attempt a standing tackle |

**Without the ball, AI manages your footballer's positioning.** You can request a challenge by tapping an opposing player; normal pitch taps do not take over off-ball running.

A separate **SPRINT** reserve and **ENERGY** indicator reflect short bursts of effort and broader match fitness. Pace, acceleration, stamina and remaining energy influence movement and recovery.

### 2D matches — the core of the career

The live 2D match engine covers passing, shooting, dribbling, crossings, pressing, goalkeeper actions, goal kicks, throw-ins, corners, free kicks, penalties, offside, fouls, cards, substitutions and full-time results. Tactical formations, collective movement and player decisions affect how each side plays.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20190809.png" width="27%" alt="2D match formation and the full pitch">
<img src="media/snapshots/Screenshot%202026-10-13%20190839.png" width="27%" alt="2D football live match">
<img src="media/snapshots/Screenshot%202026-10-13%20190900.png" width="27%" alt="2D match action near the goal">
</div>

## Train for your next chance

No9 connects training to the footballer you become. The career has **three regular weekly training sessions** and a separate weekly recovery option. Drills develop different abilities while intensity, fatigue and facility quality affect your preparation.

A catalog of **20 interactive exercises** covers ball control, dribbling, passing, shooting, sprinting, crossing, defensive duels, movement without the ball, aerial play, combinations and set pieces. A dedicated training laboratory also lets you practice without changing your career rewards.

The same catalog can be explored in **native 3D training modes**, with a player, independent ball, targets, goals, support players and goalkeepers.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20184900.png" width="27%" alt="Weekly football training options">
<img src="media/snapshots/Screenshot%202026-10-13%20185202.png" width="27%" alt="Native training drill briefing">
<img src="media/snapshots/Screenshot%202026-10-13%20185232.png" width="27%" alt="Training action on the 3D pitch">
</div>

## The world of No9

No9's documented competition catalog contains:

| Football world | Included |
| :-- | --: |
| Associations with domestic competitions | **152** |
| Persistent club identities in the current database | **8,933** |
| Stadium identity records, including retained references | **9,123** |
| FIFA federations represented for national-team competitions | **211** |

The leagues span **Europe, Africa, Asia, North & Central America, South America and Oceania**. Some countries use a single division; others have two or three active levels, regional groups, multiple stages, championship and relegation splits, or promotion play-offs. Structures vary with the league rather than forcing every country into the same formula.

The football calendar also supports national cups, international club competitions and national-team tournaments: European club football, Libertadores and Sudamericana, North and Central American competitions, Asian and African continental tournaments, Oceanian club football, continental championships and the World Cup.

**Competition formats are adapted to the game's calendar and available club catalog.** Club names and competition references do not imply official affiliation, endorsement or licensing.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20185019.png" width="27%" alt="Worldwide football, nations and competitions">
<img src="media/snapshots/Screenshot%202026-10-13%20185032.png" width="27%" alt="Selecting international football competitions">
<img src="media/snapshots/Screenshot%202026-10-13%20185051.png" width="27%" alt="European club competition fixtures">
</div>

## Beyond the touchline

A football career is more than match results. No9 includes a phone, an agent, messages, clubs, training facilities, schedules, equipment, profile and statistics, plus city services and leisure activities. The aim is for your decisions and achievements between matches to feel connected to the player you become on the pitch.

## Native 3D football and player development

The native Godot 3D environment now serves both **official career fixtures** and separate development/training scenes. It contains the Solv3 player with a customizable kit, football actions, team movement, goalkeeper play, the training catalog, stadium environments and demonstration football. Official results share the existing career simulation and save path; the training and animation showcases remain clearly marked as development facilities.

### The player

The current 3D player pipeline uses the Solv3 model prepared in Blender, football kit and a shared catalog of 130 authorized/native animation clips. Player, goalkeeper, referee and coach roles have separate presentation requirements. The dedicated showcase includes movements, passes, shots, headers, challenges, goalkeeper actions and celebrations.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20183822.png" width="30%" alt="Native 3D player wearing training kit">
<img src="media/snapshots/Screenshot%202026-10-13%20183840.png" width="30%" alt="Football shirt name and number">
<img src="media/snapshots/Screenshot%202026-10-13%20183947.png" width="30%" alt="3D player controlling a football">
</div>

### The training grounds

Five training-base configurations range from a single small pitch to multi-pitch campuses with changing rooms, training buildings, facilities and outdoor environments. Some include a sports hall or a swimming pool. Park-style and mountain stadium environments add surroundings, access roads, fences and match-day facilities.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20183356.png" width="44%" alt="Training campus and swimming pool">
<img src="media/snapshots/Screenshot%202026-10-13%20185334.png" width="44%" alt="Aerial overview of the football academy">
</div>

### Football, stadiums and match presentation

Native 3D demonstrations include **5+1 small-sided play** and **11-versus-11 friendly play** with match officials, arrivals, substitutions and results. **Official competitive career fixtures can now run in 3D**, with the existing AuthorityEngine and career completion flow. Separate development matches remain distinct from these official fixtures.

<div align="center">
<img src="media/snapshots/Screenshot%202026-10-13%20185646.png" width="30%" alt="Teams walking onto the pitch">
<img src="media/snapshots/Screenshot%202026-10-13%20185958.png" width="30%" alt="Native 3D match presentation">
<img src="media/snapshots/Screenshot%202026-10-13%20190115.png" width="30%" alt="Fourth official with substitution board">
</div>

## Development update — 24 October 2026

The stadium authoring library brings **124 assets and two assembly examples onto one Godot gallery page**: stands and end stands, connected corners, tier and roof options, floodlights, scoreboards, advertising, standing terraces, steel bleachers and award presentation pieces. The existing rural, urban, plain and mountain match environments remain available.

Stadium options include full or central-half canopies, seven roof shapes, three support structures, and a full single stand, two independent stands, a centered half-width stand or no stand on each side. Each of the four corners can be enabled separately. There is no roof above an absent corner. Seat palettes use **one, two or three colors** with uniform, random individual-seat mosaic, global vertical sectors, large chess blocks, ring colors or bottom-to-top fading. Mosaic and fade keep discrete seat colors at every distance; distant chairs use four triangles each rather than color-averaged strips. Floodlights face the pitch. Covered examples can mount lights beneath the roof; scoreboards include central cable suspension with no full roof, roof-edge mounting and closed niches. Advertising can use one or two rows on the pitch perimeter, on rectangular spectator fencing, or both.

<div align="center">
<img src="media/development-2026-10-23/stadium-gallery.png" width="95%" alt="All 115 stadium authoring assets together on one Godot page">
</div>

<p align="center"><img src="media/development-2026-10-23/mosaic-three-colors.png" width="95%" alt="Discrete three-color stadium seat mosaic with continuous height transitions through the curved corner"></p>

The library now includes **24 original team dugouts**: six construction families, one row of ten seats or two rows of seven seats each, at ground level or partially recessed. Recessed variants have access steps, retaining walls and real ground cutouts. The editor offers opaque or tinted transparent shelter panels, with separate seat and wall/roof colors. Finish changes update materials without rebuilding the stadium. All variants remain on the same Godot gallery page.

<p align="center"><img src="media/development-2026-10-23/dugout-curved.png" width="95%" alt="Four curved dugout variants: ground level and recessed, one and two seating rows"></p>

<p align="center"><img src="media/development-2026-10-23/dugout-finishes.png" width="95%" alt="Independent red seats and blue panels: opaque on the left, transparent on the right"></p>

### No9Editor — a separate desktop application

**No9Editor** (up to **1.2.18** in the 27 October desktop verification; the stadium authoring description below began with 1.1.13) is a standalone Windows editor with database search, readable regulations and a live 3D stadium preview. It does not require an installed Godot editor. Names, club short names, two or three identity colors, stadium assignment, home/away/optional third kit colors, stadium capacity and appearance are editable. Stadiums can be searched by name or created without rewriting the base catalogs. Rules, ratings, memberships and identifiers are protected.

Selecting a league shows its name and the **clubs registered in the catalog's current season**. Regulations are presented as paragraphs rather than code. The international competition browser separates **17 club competitions and seven national-team competitions**. The game's Champions League, Europa League and Conference League each use groups of eight, with seven matches per club: one match against each opponent, without a group-stage return leg.

Existing surroundings are selected by **Town/Village/Metropolitan**, **Plain/Mountain** and one of **42 stadium environment templates**, adapted to the stadium footprint. The selector uses dropdowns without a reference photograph. Parking stays at its authored baseline, then adds one space per full 100 seats above 500, in elongated rows. Suspended scoreboards scale with stadium capacity.

The stadium preview reuses the basic stadium's actual playing surface, markings, corner flags and both goals with nets. It adds configurable stands around the pitch and provides the touchline space needed for the selected dugouts. Coach figures are hidden in the editor preview. Changing a venue no longer leaves another stadium on screen after an invalid selection. Incompatible edits restore the last valid configuration and show their reason above the preview. These settings remain stadium authoring and database configuration; they do not automatically replace every existing 3D match scene.

The new rear-access option is available for single-ring stadiums: broad external stairs climb planted embankments to the continuous top promenade. Rear stairs now continue through every constructed corner, aligned with the interior aisles. Other choices include base entries, base entries below forty rows, centered entries at forty to forty-nine rows and entries at rows 20, 40, 60 and onward for rings with at least fifty rows, a raised 2.4-metre stand base and independent corners without adjacent end stands. Manual side capacities retain an unfinished draft while the total is being completed. A closer camera and WASD free view make interior inspection easier. Dugout seat and panel colors use two compact adjacent controls.

<p align="center"><img src="media/development-2026-10-23/rear-access-single-ring.png" width="95%" alt="Single-ring stadium prototype with external stairs on green embankments and a continuous upper promenade"></p>

<p align="center"><img src="media/development-2026-10-23/raised-base-open-corners.png" width="95%" alt="Raised stand base and independent curved corners without adjoining end stands"></p>

Seat colors include a random individual-seat mosaic across the entire stand and a separate fade that changes the proportions of whole colored seats from bottom to top. Individual ring colors, global vertical sectors with a maximum of twelve broad equal blocks, and large chess blocks continue across corners. Seven roof shapes include external cantilevers and a ribbed membrane, with visible support structures. All six dugout families have fully enclosed backs and sides, with opaque or transparent panels. Digital advertising scrolls across adjoining cabinets as one continuous display; double rows can show independent bands or complementary halves of one tall message, preserving their physical dimensions. Combined rows align against a common camera projection plane.

<p align="center"><img src="media/development-2026-10-24/vertical-sectors-reference.png" width="95%" alt="Broad equal vertical seat sectors continuing across stadium tiers"></p>
<p align="center"><img src="media/development-2026-10-24/roof-5-independent.png" width="48%" alt="Independent canopy with visible exterior cantilever ribs"> <img src="media/development-2026-10-24/roof-6-continuous.png" width="48%" alt="Continuous ribbed membrane roof around the stadium"></p>

The editor offers **42 stadium environments**, selected by **town, village or metropolitan area**, then **plain or mountain**. Each of the three settlement types has seven plain and seven mountain variants. Training facilities are excluded from these 42 stadium choices. The original perimeter street is retained in all 42 surroundings, with different building programmes and frontage arrangements rather than palette swaps. Compact neighborhoods include gardens, parks, balconies, varied roof shapes and buildings up to twenty floors. As the stadium footprint expands, additional complete buildings populate the lengthened street frontages to preserve neighbourhood density. Hundreds of trees use several realistic broadleaf models, with additional conifers and sparse dead trees in mountain environments. Close trees retain their 3D meshes; distant forests use four-view, two-triangle representations. Roads, sidewalks, parking and door approaches are checked for obstruction. Natural ground and rock textures replace the repeating painted squares on hills.

The additional Mowed Grass 3D layer has been removed at the user's request. The original playing surface, colors and material remain unchanged. The base selector offers ground level with a fence, ground level with a low wall, or a 2.4 m raised base with a low wall and the standard walkway. Between-ring separation keeps its standard small wall. An independent protection switch applies only to spectator-entry walkways within the same ring. Public-bench spectators now sit on the seat with their feet down. Existing and added civilian vehicle models are used together; the rejected pickup and trailer are excluded.

<p align="center"><img src="media/development-2026-10-24/comparison-urban-plain.jpg" width="95%" alt="Seven different town layouts on plains, rendered in Godot"></p>
<p align="center"><img src="media/development-2026-10-24/comparison-metropolitan-plain.jpg" width="95%" alt="Seven different metropolitan layouts on plains, rendered in Godot"></p>
<p align="center"><img src="media/development-2026-10-24/119-metropolitan-mountain.png" width="48%" alt="Metropolitan mountain environment"> <img src="media/development-2026-10-24/119-village-plain.png" width="48%" alt="Village on a plain with gardens and mixed broadleaf trees"></p>
<p align="center"><img src="media/development-2026-10-24/119-seats-1.png" width="48%" alt="Random mosaic of discrete colored seats"> <img src="media/development-2026-10-24/119-seats-6.png" width="48%" alt="Fade through changing proportions of whole colored seats"></p>
<p align="center"><img src="media/development-2026-10-24/spectators-seated.png" width="95%" alt="Basic-stadium spectators seated on the bench, with their feet below the seat"></p>

Stadiums below 100 capacity remain basic grounds. Environment, lighting and dugouts can be changed; increasing capacity to at least 100 unlocks stand construction. Colour controls share the same size and style throughout the editor.

Changes are saved as **independent update packs**, separate from the original database. Club and stadium changes from different authors can be combined, enabled, disabled and reordered. Conflicting changes to the same field use the last active pack and are reported. The database uses numeric entity IDs throughout its records and references, with **23,821 globally reserved numbers**. Stadiums with the same name in the same country share one identity, even if city information is incomplete. Older numeric IDs remain compatible redirects; names in different countries stay separate. Training grounds are excluded from the stadium editor.

<div align="center">
<img src="media/development-2026-10-24/no9editor-113.png" width="95%" alt="No9Editor 1.1.13 standalone application: a development configuration, not a reconstruction of the named real stadium">
<img src="media/development-2026-10-22/league-current-season.png" width="95%" alt="League name and the clubs included in the selected current season">
<img src="media/development-2026-10-22/rules-readable.png" width="95%" alt="League regulations presented as readable paragraphs">
<img src="media/development-2026-10-22/international-competitions.png" width="95%" alt="International club competition with seven group games and integer point totals">
</div>

### Match presentation and animation checks

The fourth official has newly authored board-carrying and board-raising poses, with bent elbows and hands gripping the lower corners. Match corrections cover close-range tackles, goalkeeper recovery after a dive, substitute bib removal, a continuous second-half ball placement and gait transitions between the authorized Solv3 clips.

<div align="center">
<img src="media/development-2026-10-22/fourth-official.png" width="32%" alt="Fourth official holding the substitution board above his hands">
<img src="media/development-2026-10-22/match-720p.png" width="32%" alt="720 by 1280 portrait 3D match development capture">
<img src="media/development-2026-10-22/match-1080p.png" width="32%" alt="1080 by 1920 portrait 3D match development capture">
</div>

The editor renders its 3D preview on demand and keeps repeated seat geometry batched. Colors and installations update without rebuilding unrelated seating. Silent background verification covers the desktop interface, the exported application, numeric references and the actual seven-round group schedules. The portrait match captures were made on Windows at **720 × 1280** and **1080 × 1920**; they are desktop development evidence, not Android or iPhone performance certification.

## Official game snapshots

The historical collection below comes from the **original No9 game/project snapshots** captured on 13 October 2026. **Eleven more media files from 25–27 October**, including two action GIFs, appear in the [latest milestone](#latest-game-milestone--27-october-2026) above. Its **40 PNG files** were copied from the game's snapshot collection into this public repository, without replacing them with mock-ups, AI-generated samples or unrelated demonstrations. The snapshots include both the career's 2D interface and the dedicated 3D development modes.

<details>
<summary><strong>Career, tactics and the football world — 8 screenshots</strong></summary>

<table>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20184846.png" width="360" alt="Player profile and attributes"><br><sub>Player profile and attributes</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20184900.png" width="360" alt="Individual training choices"><br><sub>Individual training choices</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20184915.png" width="360" alt="Team tactical setup"><br><sub>Team tactical setup</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20184932.png" width="360" alt="Club fixtures and career calendar"><br><sub>Club fixtures and career calendar</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185019.png" width="360" alt="World football and national teams"><br><sub>World football and national teams</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185032.png" width="360" alt="International competitions"><br><sub>International competitions</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185051.png" width="360" alt="European club competition fixtures"><br><sub>European club competition fixtures</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185133.png" width="360" alt="Match loading and on-screen guidance"><br><sub>Match loading and on-screen guidance</sub></td></tr>
</table>

</details>

<details open>
<summary><strong>Matchday — the 2D career pitch — 3 screenshots</strong></summary>

<table>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190809.png" width="360" alt="Matchday from kick-off"><br><sub>Matchday from kick-off</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190839.png" width="360" alt="Team shape and ball movement"><br><sub>Team shape and ball movement</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190900.png" width="360" alt="Live match action near goal"><br><sub>Live match action near goal</sub></td><td></td></tr>
</table>

</details>

<details>
<summary><strong>The footballer in native 3D — 4 screenshots</strong></summary>

<table>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183822.png" width="360" alt="Player model, front view"><br><sub>Player model, front view</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183840.png" width="360" alt="Jersey number and player name"><br><sub>Jersey number and player name</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183919.png" width="360" alt="Player movement"><br><sub>Player movement</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183947.png" width="360" alt="Ball mastery and close control"><br><sub>Ball mastery and close control</sub></td></tr>
</table>

</details>

<details>
<summary><strong>Interactive 3D training and match presentation — 16 screenshots</strong></summary>

<table>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185202.png" width="360" alt="Training briefing"><br><sub>Training briefing</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185232.png" width="360" alt="On-pitch training"><br><sub>On-pitch training</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185351.png" width="360" alt="Full-size demonstration match"><br><sub>Full-size demonstration match</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185426.png" width="360" alt="Training in rainy conditions"><br><sub>Training in rainy conditions</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185646.png" width="360" alt="Teams walking onto the pitch"><br><sub>Teams walking onto the pitch</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185653.png" width="360" alt="Pre-match line-up"><br><sub>Pre-match line-up</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185715.png" width="360" alt="Players getting ready"><br><sub>Players getting ready</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185728.png" width="360" alt="Match official"><br><sub>Match official</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185855.png" width="360" alt="Goal celebration"><br><sub>Goal celebration</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185952.png" width="360" alt="Football in the rain"><br><sub>Football in the rain</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185958.png" width="360" alt="Wide view of live 3D action"><br><sub>Wide view of live 3D action</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190115.png" width="360" alt="Substitution board"><br><sub>Substitution board</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190131.png" width="360" alt="Player coming on"><br><sub>Player coming on</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190148.png" width="360" alt="Teams on the pitch"><br><sub>Teams on the pitch</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190248.png" width="360" alt="Live ball action"><br><sub>Live ball action</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20190456.png" width="360" alt="Post-match statistics"><br><sub>Post-match statistics</sub></td></tr>
</table>

</details>

<details>
<summary><strong>Training grounds, facilities and stadium surroundings — 9 screenshots</strong></summary>

<table>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20181459.png" width="360" alt="Training base, field-side paths"><br><sub>Training base, field-side paths</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183246.png" width="360" alt="Playing fields and parking"><br><sub>Playing fields and parking</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183327.png" width="360" alt="Pitch, hills and surroundings"><br><sub>Pitch, hills and surroundings</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183356.png" width="360" alt="Swimming pool and football campus"><br><sub>Swimming pool and football campus</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183421.png" width="360" alt="Football goals and fencing"><br><sub>Football goals and fencing</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183527.png" width="360" alt="Car park and adjacent grounds"><br><sub>Car park and adjacent grounds</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20183654.png" width="360" alt="Practice pitches and pathways"><br><sub>Practice pitches and pathways</sub></td><td align="center"><img src="media/snapshots/Screenshot%202026-10-13%20185334.png" width="360" alt="Sports academy campus seen from above"><br><sub>Sports academy campus seen from above</sub></td></tr>
<tr><td align="center"><img src="media/snapshots/bench-snap.png" width="360" alt="Benches, parking and landscape"><br><sub>Benches, parking and landscape</sub></td><td></td></tr>
</table>

</details>

## Where the journey leads

The long-term goal is a footballer's life that feels connected from the first trial to the biggest matches: a living competitive world, meaningful player growth and a match experience driven by football logic.

Next priorities include validating the now-connected official 3D match flow on actual Android devices, refining player and goalkeeper motion, improving match atmosphere and stadium life, extending contracts and club relationships, and measuring loading times, frame pacing and battery demands on real hardware.

**Current status:** active development. The Godot project currently has an Android export configuration; **iOS is a target platform**, not an announced or verified public release. The existence of development scenes and screenshots does not establish a completed mobile build.

## Public builds

Follow the [Footballer Releases page](https://github.com/florinhangu/Footballer/releases) for public APKs when they are published. The release page is the authoritative place to check availability; a snapshot or feature description is not proof of an available download.

---

## Credits

**Created and directed by Florin Hangu.** ChatGPT and Codex have assisted with research, implementation and development iteration.

No9 is built with [Godot Engine](https://godotengine.org/) and benefits from open-source tools, assets and community work. Credits and licensing information are documented in the [full Credits & Attribution](docs/CREDITS.md).

| Contributor / community | Contribution |
| :-- | :-- |
| [Godot Engine](https://godotengine.org/) and its contributors | Game engine, scripting and runtime |
| Elissa Moeller and the [Humanizer community](https://github.com/NitroxNova/humanizer) | Native character creation tooling |
| [MakeHuman Community](https://www.makehumancommunity.org/) | Related character ecosystem and resources |
| [Quaternius](https://quaternius.com/) | Nature and environment assets |
| [Poly Haven](https://polyhaven.com/) | Natural textures and reference assets |
| [Poly Pizza](https://poly.pizza/) and individual pack creators | Environmental models and props |
| [Kenney](https://kenney.nl/), Rgsdev and other asset creators | Modular scenery and vehicles |
| [Tabler Icons](https://github.com/tabler/tabler-icons) and [Flag Icons](https://github.com/lipis/flag-icons) contributors | Icons and flag resources |
| Independent music, sound-effect and font creators | Soundtrack, football atmosphere, interface and kit typography |

Individual asset licenses and any additional attribution requirements remain applicable. Trademarks and organization names belong to their respective owners; No9 is an independent project and is not officially licensed or endorsed by those football bodies.

## Thanks

Thanks to the Godot and football-game-development communities, open-source maintainers, artists, testers and everyone sharing expertise that makes independent game development possible. And thanks to everyone following the project and helping shape the football experience.

**Your first contract is only the beginning.**

<p align="center"><img src="media/development-2026-10-24/team-stadium-kit-options.png" width="95%" alt="Club stadium assignment and independent shirt, shorts and socks colors"></p>
