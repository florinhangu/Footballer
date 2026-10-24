# Credits & Thanks

No9: Day One is created and directed by **Florin Hangu**, with **ChatGPT and Codex** assisting development, research and creative iteration.

Thank you to the people who share their work with the game-development community. The credits below were checked against bundled licenses, Godot plugin metadata, asset source records and upstream project pages on 12 October 2026.

## Engine and development support

- **Godot Engine** — Juan Linietsky, Ariel Manzur and the [Godot contributors](https://github.com/godotengine/godot). [MIT notice](licenses/godot-MIT.txt).
- **ChatGPT and Codex** — [OpenAI](https://openai.com/), used for development assistance. Godot is the runtime engine; these tools are credited for their role in making the project.

## Characters, environment assets and interface resources

Environment additions reviewed on 24 October 2026:

- **Trees & Bushes** — Painkiller5555, [source](https://www.blendswap.com/blends/view/78071), CC BY 3.0. Adapted into six reduced broadleaf and three bush models.
- **Realistic Forest with Cycles** — Blenderudit, [source](https://www.blendswap.com/blends/view/70773), CC BY 3.0. Bark texture adapted for reduced foliage.
- **Mowed Grass – Cycles** — jefftml, [source](https://www.blendswap.com/blends/view/77438), CC BY 3.0. Combed particle paths adapted into 1.6 cm curved near-view blades and a distant surface texture.

These descriptions record modifications; the public presentation repository contains screenshots, not the raw source packs.

| Resource | Creator / origin | License evidence |
| --- | --- | --- |
| Humanizer addon | Elissa Moeller; [NitroxNova/Humanizer](https://github.com/NitroxNova/humanizer); bundled plugin version 2.2.0 | [Unlicense](licenses/humanizer-Unlicense.txt) for addon code |
| MakeHuman / MPFB body and equipment | [MakeHuman Community](https://www.makehumancommunity.org/), Data Collection AB, Joel Palmius, Jonas Hauquier | Inspected mesh headers declare CC0; material notices need separate treatment, below |
| Stylized Nature MegaKit Standard | [Quaternius](https://quaternius.com/); Godot Asset Store package | [CC0 1.0](licenses/quaternius-CC0.txt) |
| Nature & Terrain — Free Edition | [Avramania](https://www.avramania.com/); Nature_Terrain_Free archive | [CC0 1.0](licenses/avramania-CC0.txt) |
| Free 3D Modular Game Assets for Prototyping | Raphael Gonçalves / [Rgsdev](https://www.patreon.com/rgsdev) | [CC0](licenses/rgsdev-prototyping-CC0.txt) |
| Free Low Poly Vehicles Pack | Raphael Gonçalves / Rgsdev | [CC0](licenses/rgsdev-vehicles-CC0.txt) |
| Stylized Grass meshes / shader | [StayAtHomeDev](https://stayathomedev.itch.io/stylized-grass-shader); stylizedGrassMeshes and shaderSTYLIZEDGRASS archives | [MIT](licenses/stylized-grass-MIT.txt), identical notice in both folders |
| Tabler Icons | Paweł Kuna and [Tabler contributors](https://github.com/tabler/tabler-icons) | [MIT](licenses/tabler-MIT.txt) |
| Flag Icons | Panayiotis Lipiridis and [flag-icons contributors](https://github.com/lipis/flag-icons) | [MIT](licenses/flag-icons-MIT.txt), also retained with the documentation flags |
| A_R7 vehicle asset | A_R7 archive; creator not named in the inspected source record or notice | [CC0 notice](licenses/a-r7-CC0.txt); individual attribution remains unresolved |

Acknowledgement records inclusion in the development repository. It does not mean every tool or asset is active in every scene or included in a public APK. The current native character work is Humanizer-based; old Lunin/Mesh2Motion experiments are not presented as the current pipeline.

## MakeHuman asset-specific notices

Inspected source headers include:

| Source asset | Recorded information |
| --- | --- |
| DefaultBody.mhclo | CC0; generated using MPFB2 |
| Young Caucasian Male material | Explicit CC0 release in September 2020; Data Collection AB, Joel Palmius and Jonas Hauquier |
| Hair-Short02.mhclo | Explicit CC0 release in September 2020; the same named rights holders |
| Shoes-02.mhclo | Explicit CC0 release in September 2020; the same named rights holders |
| Shirt-MakeHumanTShirt.mhclo | CC0; author field explicitly says “unknown” |
| bogdan666_short_02_gray.mhmat | Bundled header names Data Collection AB, Joel Palmius and Jonas Hauquier and still says AGPLv3 |

The gray-hair material notice differs from the CC0 notices on the inspected meshes. Its [original header](licenses/humanizer-gray-material-notice.txt) is preserved separately. The name “bogdan666” in its filename does not, by itself, verify the creator of that material. These entries record the evidence found; they do not assign one license to the entire MakeHuman asset collection.

Source locations in the private development tree:

- addons/humanizer/data/assets/equipment/body/Default/
- addons/humanizer/data/assets/equipment/hair/short02/
- addons/humanizer/data/assets/equipment/outfits/female_casualsuit01/
- addons/humanizer/data/assets/equipment/shoes/shoes02/

## Fonts

| Font | Copyright attribution in bundled notice | Notice |
| --- | --- | --- |
| Bebas Neue | Dharma Type, 2010 | [SIL OFL 1.1](licenses/bebasneue-OFL.txt) |
| Anton | The Anton Project Authors, 2020; [upstream](https://github.com/googlefonts/AntonFont) | [SIL OFL 1.1](licenses/anton-OFL.txt) |
| Oswald | The Oswald Project Authors, 2016; [upstream](https://github.com/googlefonts/OswaldFont) | [SIL OFL 1.1](licenses/oswald-OFL.txt) |
| Barlow Condensed | The Barlow Project Authors, 2017; [upstream](https://github.com/jpt/barlow) | [SIL OFL 1.1](licenses/barlowcondensed-OFL.txt) |
| Rajdhani | Indian Type Foundry, 2014 | [SIL OFL 1.1](licenses/rajdhani-OFL.txt) |

These are the local jersey-font assets.

## Editor and development tools

| Tool | Creator / origin | License |
| --- | --- | --- |
| Road Generator | Moo-Ack! Productions / TheDuckCow; [source](https://github.com/TheDuckCow/godot-road-generator) | [MIT](licenses/road-generator-MIT.txt) |
| RichText3D | Matias Szylkowski; [source](https://github.com/mszylkowski/rich-text-3d-godot) | [MIT](licenses/richtext3d-MIT.txt) |
| Material Layers | Foyezes; [source](https://github.com/Foyezes/Godot-Material-Layers-Legacy) | [MIT](licenses/material-layers-MIT.txt) |
| Ragdoll Generator | Manik Sharma; [source](https://github.com/Manik2607/auto-ragdoll) | [MIT](licenses/ragdoll-generator-MIT.txt) |
| Low Poly Terrain Builder | Fabian S / 78sForge; [source](https://github.com/78sForge/LowPolyTerrainBuilder) | [MIT](licenses/low-poly-terrain-MIT.txt) |
| M.A.V.S / Advanced Vehicle System | Millu30, also credited as Gidan; [source](https://github.com/Dente222/MAdvanced-Vehicle-Controller) | [MIT](licenses/mavs-MIT.txt) |
| Weather System (Lite) | Sean Elovirta; creator confirmed by bundled plugin metadata and license | [MIT](licenses/weather-lite-MIT.txt) |

The source URLs for Material Layers, Ragdoll Generator, Low Poly Terrain Builder and M.A.V.S are recorded by the project's addon-vendoring workflow. A verified separate upstream URL for Weather System (Lite) was not found, so none is invented.

## Logos

- **Godot logo** — © 2017 Andrea Calabró, [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). [Original notice](../media/branding/GODOT-LICENSE.txt); official [Godot press kit](https://godotengine.org/press/).
- **ChatGPT logo and marks** — OpenAI. Image obtained from the [official OpenAI Help Center](https://help.openai.com/en/articles/7905742-what-does-the-official-chatgpt-ios-app-icon-look-like); use governed by the [OpenAI brand guidelines](https://openai.com/brand/).

The logos are linked acknowledgements of tools used in development, not a sponsorship statement. Both are stored unmodified in this repository.

## No9 work and screenshots

Career systems, competition integration, project-specific geometry, football presentation, shaders and interface work are credited to the No9 project and its development process. Third-party portions keep their own attribution.

The screenshots are existing No9 development captures selected for this page. [Provenance and dates](../media/README.md) identify the source files. No license to the private game source is granted by publishing the screenshots.

Club and competition names do not imply affiliation or endorsement.

The copied notices document what was inspected; they are not a complete list of every dependency that a future APK may ship.
