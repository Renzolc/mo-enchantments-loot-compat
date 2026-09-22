## Mo' Enchantments Loot Compat

Makes **Mo' Enchantments** appear in the **enchanting table** and **random loot**, not only villager trades.

### The problem
Mo' Enchantments registers its enchantments for librarians (`#minecraft:tradeable`) but does not add them to the enchanting-table or loot tags. With mods like All Enchantments For Trade, they show up in trades — and nowhere else.

### What this does
Adds every Mo' Enchantments enchantment to:
- `#minecraft:non_treasure` — enchanting table
- `#minecraft:on_random_loot` — chest / loot books
- `#minecraft:tradeable` — keeps trades working

Also clears Mo' Enchantments' treasure-only lock so enchants like Rebirth / Homing aren't stuck as treasure-only.

### Requirements
- Minecraft **1.21.1**
- **NeoForge** 21.1.x
- **Mo' Enchantments**

### License
**MIT**

Not affiliated with Mo' Enchantments; a small community datapack-in-a-jar compat.
