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

4. Launch. Every mod installs itself, and re-syncs on every launch from then on.
   There are no manual steps.

## What is in here

Progression: ProjectE, Lucky Block, Baubles, Trinkets and Baubles, Bauble of Undying.

Threat: Scape and Run: Parasites + NoCube's Nests addon.

World: Modern Ruins Pack (with Chisel + CTM).

Rules: Corpse Complex (baubles stay in your inventory when you die, nothing else does),
Soulbound (custom, treasure enchantment from villager trades and chest loot, and it
applies to *any* item on an anvil, including durability-less modded ones like the
ProjectE Transmutation Tablet),
StarterKits (everyone spawns with 5 lucky blocks, iron gear, 2 soulbound books, 10 bread).

`Soulbound-1.12.2-1.0.1.jar` is shipped in this repo directly, it is not a CurseForge mod.
It is built from `~/mc-mods/soulbound`.
