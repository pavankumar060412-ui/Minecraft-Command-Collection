# Useful Minecraft Commands

A collection of helpful Minecraft commands for survival, building, and everyday gameplay.

## Teleport Player

```mcfunction
/tp <player> <x> <y> <z>
```

Example:
```mcfunction
/tp Steve 100 64 -200
```

## Change Weather

```mcfunction
/weather clear
```

## Change Time

```mcfunction
/time set day
```

## Give Items

```mcfunction
/give @p <item> <amount>
```

Example:
```mcfunction
/give @p diamond 64
```

## Change Game Mode

```mcfunction
/gamemode creative
```

## Kill Entities

```mcfunction
/kill @e[type=<mob>]
```

## Locate Structures

```mcfunction
/locate structure <structure_name>
```

## Set World Spawn

```mcfunction
/setworldspawn
```

## Set Spawn Point

```mcfunction
/spawnpoint
```

## Change Difficulty

```mcfunction
/difficulty peaceful
```

## Summon Mobs

```mcfunction
/summon <entity>
```

Example:
```mcfunction
/summon minecraft:warden
```

## Clear Inventory

```mcfunction
/clear
```

## Enchant Items

```mcfunction
/enchant @p <enchantment> <level>
```

Example:
```mcfunction
/enchant @p sharpness 5
```

## Add Experience

```mcfunction
/xp add @p <amount> levels
```

Example:
```mcfunction
/xp add @p 10 levels
```

## Weather Types

Rain:
```mcfunction
/weather rain
```

Thunderstorm:
```mcfunction
/weather thunder
```

## Freeze Time

```mcfunction
/gamerule doDaylightCycle false
```

## Keep Inventory After Death

```mcfunction
/gamerule keepInventory true
```

## Show Coordinates

```mcfunction
/gamerule showCoordinates true
```

---

More commands and guides will be added over time.
