# Vellum skins

Skins for [Vellum Game Launcher](https://github.com/cschanbusch/vellum) that are published
separately from Vellum's own releases: the showcase skins.

| Skin | Style |
| --- | --- |
| Grand Tour | An early-2000s racing showroom: a Garage view where every game gets a 3D case on a turntable, with wear and tear, a pit-service minigame and synthesized engine sounds |
| Frontier | Smoke, brush strokes and wood type (fan-made, in the style of Red Dead Redemption 2), with a Catalogue view: the library as a mail-order book you page through |
| FICSIT Terminal | An industrial library terminal (fan-made, in the style of Satisfactory) |
| Calling Card | Red, black and white menus with ransom-note type (fan-made, in the style of Persona 5) |

The fan-made skins use no original game assets and aren't affiliated with or endorsed by the
games' publishers.

## Installing

**In Vellum 0.2.1 or newer:** Settings → **Get skins**. Pick a skin and a version and choose
**Download**; then activate it in Settings → Skins. Updates, older versions and removal are on the
same page.

**By hand (any version):** download a skin's zip from [Releases](../../releases) and extract it
into the `plugins\skins` folder at the top of your Vellum folder (create it if it's missing), so
you get `plugins\skins\<skin>\plugin.json`. Then choose **Reload plugins** in Settings → Plugins,
or restart Vellum.

## Licence

These skins are **source-available, not open source**. Each zip carries its licence
(`LICENSE.md`): PolyForm Strict 1.0.0, plus permission to change a skin for your own use. You may
use them with Vellum and learn from them, but you may not redistribute them, or modified
versions, without written permission. Third-party parts (fonts, three.js) keep their own
licences, noted in each skin.

To ask for permission: Charles Schanbusch, charlieschanbusch@gmail.com, or @orcinusprime on
Discord.

## How the catalog works

`catalog.json` lists each skin and its versions; Vellum reads it from this repository. Each
version is a release tagged `<skin id>-v<version>` with the skin's zip (one folder named after the
skin's id) and a preview image. The catalog gives each zip's size and SHA-256, which Vellum checks
after downloading. Releases are published with `scripts/publish-skins.mjs` in the Vellum
repository; the skins' source lives there, under `extras/skins/`.
