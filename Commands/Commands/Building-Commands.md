# Minecraft Building Commands

A collection of useful Minecraft commands to help builders create, edit, and manage amazing structures faster.

# Basic Building Commands

## Place a Block

```mcfunction
/setblock <x> <y> <z> <block>
```

Example:

```mcfunction
/setblock ~ ~ ~ stone
```

## Fill an Area

```mcfunction
/fill <x1> <y1> <z1> <x2> <y2> <z2> <block>
```

Example:

```mcfunction
/fill 0 64 0 10 70 10 stone
```

## Replace Blocks

```mcfunction
/fill <x1> <y1> <z1> <x2> <y2> <z2> <new_block> replace <old_block>
```

Example:

```mcfunction
/fill 0 64 0 20 70 20 glass replace stone
```

# Copy and Move Builds

## Clone a Structure

```mcfunction
/clone <x1> <y1> <z1> <x2> <y2> <z2> <destination>
```

Example:

```mcfunction
/clone 0 64 0 20 80 20 100 64 100
```

## Move a Structure

```mcfunction
/clone <area> <destination> move
```

# Builder Tools

## Get a Command Block

```mcfunction
/give @p command_block
```

## Get a Structure Block

```mcfunction
/give @p structure_block
```

## Get a Barrier Block

```mcfunction
/give @p barrier
```

## Get Light Blocks

```mcfunction
/give @p light
```

# World Editing Commands

## Clear Large Areas

```mcfunction
/fill <coordinates> air
```

Example:

```mcfunction
/fill 0 0 0 100 100 100 air
```

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

# Shape Building

## Make a Hollow Box

```mcfunction
/fill <coordinates> <block> hollow
```

Example:

```mcfunction
/fill 0 60 0 20 80 20 stone hollow
```

## Make a Box Outline

```mcfunction
/fill <coordinates> <block> outline
```

## Replace Only Certain Blocks

```mcfunction
/fill <coordinates> <block> replace <old_block>
```

# Decoration Commands

## Give Armor Stand

```mcfunction
/give @p armor_stand
```

## Invisible Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Invisible:1b}
```

## Floating Text Using Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {CustomName:'{"text":"Your Text"}',Invisible:1b,CustomNameVisible:1b}
```

# Builder Game Mode

## Switch To Creative

```mcfunction
/gamemode creative
```

## Fly Faster (Using Effects)

```mcfunction
/effect give @p speed 9999 5
```

## Remove Fall Damage

```mcfunction
/effect give @p slow_falling 9999 1
```

# Terrain Commands

## Create Mountains

```mcfunction
/fill <area> stone
```

## Create Water Areas

```mcfunction
/fill <area> water
```

## Create Lava Areas

```mcfunction
/fill <area> lava
```

# Building Tips

- Use `/fill` for large walls, floors, and landscapes.
- Use `/clone` to duplicate buildings quickly.
- Use `/setblock` for precise placement.
- Use structure blocks to save and load builds.
- Always test large commands in a backup world.

---

More building commands, tutorials, and advanced construction techniques will be added over time.
