# Minecraft Target Selector Guide

A complete guide to Minecraft target selectors used to choose players and entities for commands.

# What Are Target Selectors?

Target selectors allow commands to choose specific players or entities without typing their names.

Example:

```mcfunction
/give @p diamond
```

`@p` selects the nearest player.

---

# Basic Target Selectors

## Nearest Player

```mcfunction
@p
```

Selects the closest player.

Example:

```mcfunction
/give @p diamond
```

---

## All Players

```mcfunction
@a
```

Selects every player.

Example:

```mcfunction
/effect give @a speed 10 1
```

---

## Random Player

```mcfunction
@r
```

Selects a random player.

Example:

```mcfunction
/tp @r ~ ~10 ~
```

---

## All Entities

```mcfunction
@e
```

Selects all entities.

Example:

```mcfunction
/kill @e[type=zombie]
```

---

## Command Executor

```mcfunction
@s
```

Selects the entity running the command.

Example:

```mcfunction
/effect give @s strength 10 1
```

---

# Selector Arguments

Arguments are placed inside brackets:

```mcfunction
@e[type=zombie]
```

---

# Type Selector

Select a specific entity type.

Example:

```mcfunction
@e[type=creeper]
```

More examples:

```mcfunction
@e[type=skeleton]
```

```mcfunction
@e[type=villager]
```

---

# Distance Selector

Select entities within a distance.

Example:

```mcfunction
@a[distance=..10]
```

Selects players within 10 blocks.

Range example:

```mcfunction
@e[distance=5..20]
```

---

# Name Selector

Select by name.

Example:

```mcfunction
@e[name=Boss]
```

---

# Tag Selector

Select entities with tags.

Example:

```mcfunction
@e[tag=boss]
```

---

# Team Selector

Select players on teams.

Example:

```mcfunction
@a[team=Red]
```

---

# Gamemode Selector

Select players by gamemode.

Examples:

```mcfunction
@a[gamemode=creative]
```

```mcfunction
@a[gamemode=survival]
```

---

# Limit Selector

Limit the number of targets.

Example:

```mcfunction
@e[type=zombie,limit=1]
```

Selects one zombie.

---

# Sort Selector

Controls selection order.

Options:

```text
nearest
furthest
random
arbitrary
```

Example:

```mcfunction
@e[type=item,sort=nearest]
```

---

# Level Selector

Select players by experience level.

Example:

```mcfunction
@a[level=10]
```

Range:

```mcfunction
@a[level=10..50]
```

---

# Rotation Selector

Select players by looking direction.

Example:

```mcfunction
@a[y_rotation=0]
```

---

# Position Selectors

Select entities around coordinates.

Example:

```mcfunction
@e[x=100,y=64,z=100,distance=..5]
```

---

# Combined Selectors

Multiple arguments can be combined.

Example:

```mcfunction
@e[type=zombie,tag=boss,distance=..20]
```

Finds:
- Zombies
- With boss tag
- Within 20 blocks

---

# Advanced Examples

## Kill All Creepers Nearby

```mcfunction
/kill @e[type=creeper,distance=..20]
```

---

## Give Nearby Players Speed

```mcfunction
/effect give @a[distance=..10] speed 10 1
```

---

## Detect A Boss

```mcfunction
/execute if entity @e[tag=boss]
```

---

# Selector Tips

- Combine selectors for precise targeting.
- Use tags for custom systems.
- Use `@s` inside functions.
- Test selectors before using them in large systems.

---

More advanced selector examples will be added over time.
