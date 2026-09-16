# ChaosServer

Minecraft **1.12.2**, Forge **14.23.5.2864**. A packwiz pack.

## Setup in Prism Launcher

1. Add Instance -> Custom, Minecraft **1.12.2**, Forge **14.23.5.2864**.
2. Download [packwiz-installer-bootstrap.jar](https://github.com/packwiz/packwiz-installer-bootstrap/releases/latest/download/packwiz-installer-bootstrap.jar)
   into the instance's `.minecraft` folder.
3. Instance -> Edit -> Settings -> Custom commands -> tick "Custom commands", and set
   **Pre-launch command** to:

   ```
   "$INST_JAVA" -jar packwiz-installer-bootstrap.jar https://raw.githubusercontent.com/JefNotelteirs/ChaosServer/main/pack.toml
   ```

4. **Do the manual downloads below first** (see next section), then launch. Everything
   else installs itself, and re-syncs on every launch from then on.

## Three mods must be downloaded by hand, before the first launch

Their authors have turned off third-party API access on CurseForge, so packwiz is not
allowed to fetch them.

**This is not optional and the order matters.** If these three are missing, the installer
does not install "everything but those three", it aborts the whole run and you end up with
an empty `mods` folder. Put them in first.

Create `.minecraft/mods/` in the instance and drop these into it:

| Mod | File | Link |
| --- | --- | --- |
| Scape and Run: Parasites | `SRParasites-1.10.9.jar` (117 MB) | https://www.curseforge.com/minecraft/mc-mods/scape-and-run-parasites/files/8787918 |
| SRP Nests Addon (NoCube) | `NoCubes_SRP_Nests_Addon_3.0.0.jar` | https://www.curseforge.com/minecraft/mc-mods/scape-and-run-parasites-nests-addon-by-nocube/files/4048252 |
| Lucky Block | `lucky-block-forge-1.12.2-2.0.jar` | https://www.curseforge.com/minecraft/mc-mods/lucky-block/files/3652674 |

Filenames must match exactly, or packwiz will try to fetch them again on next launch.

## What is in here

Progression: ProjectE, Lucky Block, Baubles, Trinkets and Baubles, Bauble of Undying.

Threat: Scape and Run: Parasites + NoCube's Nests addon.

World: Modern Ruins Pack (with Chisel + CTM).

Rules: Corpse Complex (baubles stay in your inventory when you die, nothing else does),
Soulbound (custom, treasure enchantment from villager trades and chest loot),
StarterKits (everyone spawns with 5 lucky blocks, iron gear, 2 soulbound books, 10 bread).

`Soulbound-1.12.2-1.0.0.jar` is shipped in this repo directly, it is not a CurseForge mod.
