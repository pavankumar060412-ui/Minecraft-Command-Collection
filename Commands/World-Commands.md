# Minecraft World Commands

A collection of commands used to control, modify, and manage the Minecraft world.

# Time Commands

## Set Time To Day

```mcfunction
/time set day
```

## Set Time To Night

```mcfunction
/time set night
```

## Set Custom Time

```mcfunction
/time set <time>
```

Examples:

```mcfunction
/time set 1000
```

```mcfunction
/time set 18000
```

## Add Time

```mcfunction
/time add <amount>
```

---

# Weather Commands

## Clear Weather

```mcfunction
/weather clear
```

## Rain Weather

```mcfunction
/weather rain
```

## Thunderstorm

```mcfunction
/weather thunder
```

## Set Weather Duration

```mcfunction
/weather <type> <duration>
```

Example:

```mcfunction
/weather thunder 6000
```

---

# Difficulty Commands

## Peaceful Difficulty

```mcfunction
/difficulty peaceful
```

## Easy Difficulty

```mcfunction
/difficulty easy
```

## Normal Difficulty

```mcfunction
/difficulty normal
```

## Hard Difficulty

```mcfunction
/difficulty hard
```

---

# Spawn Commands

## Set World Spawn

```mcfunction
/setworldspawn
```

## Set World Spawn At Location

```mcfunction
/setworldspawn <x> <y> <z>
```

## Set Player Spawn Point

```mcfunction
/spawnpoint
```

## Set Specific Spawn Point

```mcfunction
/spawnpoint <player> <x> <y> <z>
```

---

# World Border Commands

## Show Border Information

```mcfunction
/worldborder get
```

## Set Border Size

```mcfunction
/worldborder set <size>
```

Example:

```mcfunction
/worldborder set 1000
```

## Increase Border Size

```mcfunction
/worldborder add <amount>
```

## Set Border Center

```mcfunction
/worldborder center <x> <z>
```

## Set Border Damage

```mcfunction
/worldborder damage amount <damage>
```

## Set Border Warning Distance

```mcfunction
/worldborder warning distance <distance>
```

## Set Border Warning Time

```mcfunction
/worldborder warning time <seconds>
```

---

# Gamerule World Commands

## Keep Inventory

```mcfunction
/gamerule keepInventory true
```

## Disable Mob Griefing

```mcfunction
/gamerule mobGriefing false
```

## Disable Fire Spread

```mcfunction
/gamerule doFireTick false
```

## Stop Day And Night Cycle

```mcfunction
/gamerule doDaylightCycle false
```

## Stop Weather Changes

```mcfunction
/gamerule doWeatherCycle false
```

## Disable Mob Spawning

```mcfunction
/gamerule doMobSpawning false
```

## Disable Natural Regeneration

```mcfunction
/gamerule naturalRegeneration false
```

## Disable Command Block Output

```mcfunction
/gamerule commandBlockOutput false
```

## Disable Death Messages

```mcfunction
/gamerule showDeathMessages false
```

## Enable Coordinates

```mcfunction
/gamerule showCoordinates true
```

---

# Locate Commands

## Find Structures

```mcfunction
/locate structure <structure>
```

Examples:

```mcfunction
/locate structure minecraft:stronghold
```

```mcfunction
/locate structure minecraft:village
```

## Find Biomes

```mcfunction
/locate biome <biome>
```

Example:

```mcfunction
/locate biome minecraft:desert
```

---

# World Editing Commands

## Place Blocks

```mcfunction
/setblock <x> <y> <z> <block>
```

## Fill Areas

```mcfunction
/fill <coordinates> <block>
```

## Clone Areas

```mcfunction
/clone <coordinates>
```

---

# Environment Commands

## Change Game Mode

```mcfunction
/gamemode creative
```

## Remove All Entities

```mcfunction
/kill @e
```

## Remove Dropped Items

```mcfunction
/kill @e[type=item]
```

## Stop Mob Spawning

```mcfunction
/gamerule doMobSpawning false
```

---

# World Save Commands

## Save World

```mcfunction
/save-all
```

## Save World Immediately

```mcfunction
/save-all flush
```

---

# Advanced World Commands

## Reload Data Packs

```mcfunction
/reload
```

## Enable Debug Mode

```mcfunction
/debug start
```

## Stop Debug Mode

```mcfunction
/debug stop
```

---

# World Management Tips

- Use gamerules to customize survival worlds.
- Use world borders for challenges.
- Use locate commands to find structures quickly.
- Always create backups before large world edits.
- Test powerful commands in a separate world.

---

More Minecraft world management commands and advanced features will be added over time.
