# Minecraft Building Commands

A collection of Minecraft commands and techniques designed to help builders create, edit, and manage structures faster.

# Basic Building Commands

## Place a Single Block

```mcfunction
/setblock <x> <y> <z> <block>
```

Example:

```mcfunction
/setblock ~ ~ ~ diamond_block
```

---

# Fill Commands

## Fill an Area With Blocks

```mcfunction
/fill <x1> <y1> <z1> <x2> <y2> <z2> <block>
```

Example:

```mcfunction
/fill 0 64 0 20 70 20 stone
```

## Fill Area With Air (Delete Blocks)

```mcfunction
/fill <x1> <y1> <z1> <x2> <y2> <z2> air
```

Example:

```mcfunction
/fill 0 0 0 100 100 100 air
```

## Replace Blocks

```mcfunction
/fill <coordinates> <new_block> replace <old_block>
```

Example:

```mcfunction
/fill 0 64 0 50 80 50 glass replace stone
```

## Create Hollow Structures

```mcfunction
/fill <coordinates> <block> hollow
```

Example:

```mcfunction
/fill 0 60 0 20 80 20 stone hollow
```

## Create Outline Structures

```mcfunction
/fill <coordinates> <block> outline
```

Example:

```mcfunction
/fill 0 60 0 20 80 20 quartz_block outline
```

---

# Clone Commands

## Copy Builds

```mcfunction
/clone <x1> <y1> <z1> <x2> <y2> <z2> <destination>
```

Example:

```mcfunction
/clone 0 60 0 20 80 20 100 60 100
```

## Move Builds

```mcfunction
/clone <area> <destination> move
```

## Clone Only Matching Blocks

```mcfunction
/clone <coordinates> <destination> filtered <block>
```

---

# Structure Commands

## Get Structure Block

```mcfunction
/give @p structure_block
```

## Save Structures

Use a structure block to save builds and load them later.

## Load Structures

Use structure blocks to import saved builds.

---

# Builder Tools

## Get Command Block

```mcfunction
/give @p command_block
```

## Get Repeating Command Block

```mcfunction
/give @p repeating_command_block
```

## Get Chain Command Block

```mcfunction
/give @p chain_command_block
```

## Get Barrier Blocks

```mcfunction
/give @p barrier
```

## Get Light Blocks

```mcfunction
/give @p light
```

## Get Debug Stick

```mcfunction
/give @p debug_stick
```

---

# World Editing

## Create Walls

```mcfunction
/fill <coordinates> stone
```

## Create Floors

```mcfunction
/fill <coordinates> <block>
```

Example:

```mcfunction
/fill 0 64 0 50 64 50 oak_planks
```

## Create Ceilings

```mcfunction
/fill <coordinates> <block>
```

## Remove Large Areas

```mcfunction
/fill <coordinates> air
```

---

# Terrain Building

## Create Water Area

```mcfunction
/fill <coordinates> water
```

## Create Lava Area

```mcfunction
/fill <coordinates> lava
```

## Create Mountains

Use:

```mcfunction
/fill
```

with stone, deepslate, and other blocks.

## Create Flat Areas

```mcfunction
/fill <coordinates> <block>
```

---

# Decoration Commands

## Summon Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~
```

## Invisible Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Invisible:1b}
```

## Floating Text

```mcfunction
/summon armor_stand ~ ~ ~ {CustomNameVisible:1b}
```

---

# Building Assistance

## Change To Creative Mode

```mcfunction
/gamemode creative
```

## Fly

Double jump while in creative mode.

## Night Vision For Building

```mcfunction
/effect give @p night_vision 99999 1
```

## Slow Falling

```mcfunction
/effect give @p slow_falling 99999 1
```

## Speed Boost

```mcfunction
/effect give @p speed 99999 5
```

---

# Command Block Building

## Give Command Block

```mcfunction
/give @p command_block
```

## Run Commands Automatically

Use repeating command blocks.

## Chain Commands

Use chain command blocks to run multiple commands together.

## Conditional Commands

Use conditional command blocks to make advanced systems.

---

# Building Tips

- Use `/fill` for large structures.
- Use `/clone` for copying builds.
- Use `/setblock` for precision placement.
- Use structure blocks for saving large projects.
- Always test large commands in a backup world.

---

More advanced Minecraft building commands and techniques will be added over time.
