# OreSpawn 1.20.1 (Forge) — port of OreSpawn 1.7.10

Original mod by Danger, GPL-3.0. This port keeps the GPL-3.0 license.

## Build
1. Download the **Forge 1.20.1 MDK** (47.3.0+) from files.minecraftforge.net.
2. Copy `gradlew`, `gradlew.bat` and the `gradle/` folder from the MDK into this project.
3. JDK 17 required. Then:
   - `./gradlew genIntellijRuns` (or `genEclipseRuns`) and open in the IDE
   - `./gradlew build` → jar in `build/libs/`

## Layout
- `danger.orespawn.core`  – blocks, items, sounds, creative tab
- `danger.orespawn.mobs`  – entities, AI, spawning
- `danger.orespawn.world` – dimensions, structures, ore gen
- `danger.orespawn.client`– models, renderers, GUIs
- `docs/INVENTORY.md`     – everything to port, with status
- `docs/rename_map.json`  – 1.7.10 → 1.20.1 asset renames (lowercase rule)

## Status
Stage 1 (skeleton, assets, sounds): done. Stage 2 (blocks/items): next.

## Build without installing anything (GitHub Actions)
1. Create a free GitHub account and a new empty repository.
2. Upload the contents of this folder (including the hidden `.github` folder).
3. Open the **Actions** tab, wait for "Build mod" to finish (a few minutes).
4. Open the finished run and download the **orespawn-jar** artifact, unzip it, and put the `.jar` into your `mods` folder.
