# Minecraft Loot Commands

A collection of commands used to generate, give, and manage loot in Minecraft.

# What Is The Loot Command?

The `/loot` command allows players and map creators to generate loot from loot tables, entities, blocks, and fishing.

It is useful for:
- Custom rewards
- Adventure maps
- RPG systems
- Minigames
- Random loot systems

---

# Basic Loot Command

## Give Loot To Player

```mcfunction
/loot give <player> loot <loot_table>
```

Example:

```mcfunction
/loot give @p loot minecraft:chests/simple_dungeon
```

---

# Spawn Loot

## Spawn Loot At A Location

```mcfunction
/loot spawn <x> <y> <z> loot <loot_table>
```

Example:

```mcfunction
/loot spawn ~ ~ ~ loot minecraft:chests/simple_dungeon
```

---

# Replace Inventory Items With Loot

## Replace Player Inventory Slot

```mcfunction
/loot replace entity <player> <slot> loot <loot_table>
```

Example:

```mcfunction
/loot replace entity @p weapon.mainhand loot minecraft:chests/end_city_treasure
```

---

# Loot From Entities

## Generate Mob Drops

```mcfunction
/loot give <player> kill <entity>
```

Example:

```mcfunction
/loot give @p kill @e[type=zombie,limit=1]
```

---

# Loot From Blocks

## Generate Block Drops

```mcfunction
/loot give <player> mine <block>
```

Example:

```mcfunction
/loot give @p mine minecraft:diamond_ore
```

---

# Fishing Loot

## Generate Fishing Loot

```mcfunction
/loot give <player> fish <loot_table>
```

Example:

```mcfunction
/loot give @p fish minecraft:gameplay/fishing
```

---

# Common Loot Tables

## Dungeon Chest

```text
minecraft:chests/simple_dungeon
```

## Village Weaponsmith

```text
minecraft:chests/village/village_weaponsmith
```

## Shipwreck Treasure

```text
minecraft:chests/shipwreck_treasure
```

## End City Treasure

```text
minecraft:chests/end_city_treasure
```

## Ancient City

```text
minecraft:chests/ancient_city
```

## Bastion Treasure

```text
minecraft:chests/bastion_treasure
```

## Nether Fortress

```text
minecraft:chests/nether_bridge
```

---

# Custom Reward Systems

## Random Reward Command

```mcfunction
/loot give @p loot minecraft:chests/simple_dungeon
```

Use with:
- Buttons
- Command blocks
- Scoreboards
- Advancements

---

# RPG Reward Example

When a player completes a challenge:

```mcfunction
/loot give @p loot minecraft:chests/end_city_treasure
```

Possible rewards:
- Rare items
- Enchanted equipment
- Materials
- Food
- Potions

---

# Command Block Loot Systems

## Random Loot Machine

Command block:

```mcfunction
/loot give @p loot minecraft:chests/simple_dungeon
```

Activate with:
- Buttons
- Levers
- Pressure plates

---

# Loot Ideas

Create:

- Boss rewards
- Treasure hunts
- Daily rewards
- Dungeon chests
- Custom crates
- Adventure map rewards

---

# Loot Tips

- Loot tables decide what items are generated.
- Combine loot with scoreboards for reward systems.
- Datapacks can create custom loot tables.
- Use command blocks to automate loot systems.

---

More advanced loot tables and custom reward systems will be added over time.
