# Mo' Enchantments Loot Compat (1.0.0)

NeoForge 1.21.1 datapack-in-a-jar for **Mo' Enchantments**.

## Problem
Mo' Enchantments registers its enchantments for villager trades (`#minecraft:tradeable`) but never adds them to:
- `#minecraft:non_treasure` (enchanting table)
- `#minecraft:on_random_loot` (chest / fishing / etc. enchanted books)

Its world datapack (`datapacks/MoEnchantments`) only writes `tradeable.json`.

## Fix
This mod adds **every** Mo' Enchantments enchant to:
- `#minecraft:non_treasure`
- `#minecraft:on_random_loot`
- `#minecraft:tradeable` (keeps librarian trades)

and clears `#mo_enchantments:treasure_entries` so formerly "treasure" ones (Rebirth, Homing, etc.) are not locked out of the table.

## Install
Drop `mo_enchantments_loot_compat-1.0.0.jar` in your `mods` folder next to Mo' Enchantments. Restart / create a new world session so tags reload.
