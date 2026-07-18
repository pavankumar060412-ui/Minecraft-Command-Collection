# OP Minecraft Commands

A collection of powerful Minecraft commands for operators, administrators, and players with permission to use advanced commands.

# Player Management

## Give Operator Permission

```mcfunction
/op <player>
```

## Remove Operator Permission

```mcfunction
/deop <player>
```

## Ban a Player

```mcfunction
/ban <player>
```

## Ban a Player with Reason

```mcfunction
/ban <player> <reason>
```

## Unban a Player

```mcfunction
/pardon <player>
```

## Ban an IP Address

```mcfunction
/ban-ip <ip>
```

## Remove IP Ban

```mcfunction
/pardon-ip <ip>
```

## Kick a Player

```mcfunction
/kick <player>
```

## Kick With Reason

```mcfunction
/kick <player> <reason>
```

# Teleport Commands

## Teleport Yourself

```mcfunction
/tp <x> <y> <z>
```

## Teleport Player To Coordinates

```mcfunction
/tp <player> <x> <y> <z>
```

## Teleport One Player To Another

```mcfunction
/tp <player1> <player2>
```

## Teleport Everyone To You

```mcfunction
/tp @a @s
```

# Item Commands

## Give Items

```mcfunction
/give @p <item> <amount>
```

Example:

```mcfunction
/give @p diamond_block 64
```

## Clear Inventory

```mcfunction
/clear
```

## Clear Specific Item

```mcfunction
/clear @p diamond
```

## Replace Items In Inventory

```mcfunction
/item replace entity <player> weapon.mainhand with <item>
```

# Enchantment Commands

## Add Enchantment

```mcfunction
/enchant @p <enchantment> <level>
```

Example:

```mcfunction
/enchant @p sharpness 5
```

## High Level Enchantment Example

```mcfunction
/give @p diamond_sword{Enchantments:[{id:sharpness,lvl:255}]} 1
```

# Mob Commands

## Summon Entity

```mcfunction
/summon <entity>
```

Example:

```mcfunction
/summon minecraft:warden
```

## Summon Mob At Location

```mcfunction
/summon <entity> <x> <y> <z>
```

## Kill All Mobs

```mcfunction
/kill @e[type=!player]
```

## Kill Specific Mob

```mcfunction
/kill @e[type=minecraft:zombie]
```

## Remove All Items On Ground

```mcfunction
/kill @e[type=item]
```

# Game Mode Commands

## Survival Mode

```mcfunction
/gamemode survival
```

## Creative Mode

```mcfunction
/gamemode creative
```

## Adventure Mode

```mcfunction
/gamemode adventure
```

## Spectator Mode

```mcfunction
/gamemode spectator
```

# World Commands

## Change Time

Day:

```mcfunction
/time set day
```

Night:

```mcfunction
/time set night
```

Custom Time:

```mcfunction
/time set <number>
```

## Change Weather

Clear:

```mcfunction
/weather clear
```

Rain:

```mcfunction
/weather rain
```

Thunder:

```mcfunction
/weather thunder
```

## Set World Spawn

```mcfunction
/setworldspawn
```

## Set Player Spawn

```mcfunction
/spawnpoint
```

## Change Difficulty

Peaceful:

```mcfunction
/difficulty peaceful
```

Easy:

```mcfunction
/difficulty easy
```

Normal:

```mcfunction
/difficulty normal
```

Hard:

```mcfunction
/difficulty hard
```

# Gamerule Commands

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

## Stop Daylight Cycle

```mcfunction
/gamerule doDaylightCycle false
```

## Stop Weather Cycle

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

# Effect Commands

## Give Effect

```mcfunction
/effect give <player> <effect> <seconds> <amplifier>
```

Example:

```mcfunction
/effect give @p speed 60 5
```

## Remove Effects

```mcfunction
/effect clear <player>
```

# Experience Commands

## Give XP Levels

```mcfunction
/xp add @p <amount> levels
```

Example:

```mcfunction
/xp add @p 50 levels
```

## Remove XP

```mcfunction
/xp add @p -10 levels
```

# Structure Commands

## Locate Structure

```mcfunction
/locate structure <structure>
```

Example:

```mcfunction
/locate structure minecraft:stronghold
```

## Locate Biome

```mcfunction
/locate biome <biome>
```

# World Border Commands

## Set Border Size

```mcfunction
/worldborder set <size>
```

## Add To Border

```mcfunction
/worldborder add <amount>
```

## Center Border

```mcfunction
/worldborder center <x> <z>
```

# Server Commands

## Save World

```mcfunction
/save-all
```

## Stop Server

```mcfunction
/stop
```

## Reload Data

```mcfunction
/reload
```

# Advanced Commands

## Execute Commands

```mcfunction
/execute <subcommand>
```

## Fill Area

```mcfunction
/fill <x1> <y1> <z1> <x2> <y2> <z2> <block>
```

Example:

```mcfunction
/fill 0 0 0 10 10 10 stone
```

## Clone Area

```mcfunction
/clone <x1> <y1> <z1> <x2> <y2> <z2> <destination>
```

## Set Blocks

```mcfunction
/setblock <x> <y> <z> <block>
```

Example:

```mcfunction
/setblock ~ ~ ~ diamond_block
```

## Place Structure Blocks

```mcfunction
/give @p structure_block
```

## Give Command Block

```mcfunction
/give @p command_block
```

## Give Barrier Block

```mcfunction
/give @p barrier
```

## Give Light Block

```mcfunction
/give @p light
```

---

More advanced Minecraft operator commands and tutorials will be added over time.
