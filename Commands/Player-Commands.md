# Minecraft Player Commands

A collection of commands used for managing players, abilities, inventory, movement, and player-related features.

# Teleport Commands

## Teleport Yourself

```mcfunction
/tp <x> <y> <z>
```

Example:

```mcfunction
/tp 100 64 -200
```

## Teleport Player To Location

```mcfunction
/tp <player> <x> <y> <z>
```

Example:

```mcfunction
/tp Steve 100 64 -200
```

## Teleport Player To Another Player

```mcfunction
/tp <player1> <player2>
```

Example:

```mcfunction
/tp Steve Alex
```

---

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

## Change Another Player's Game Mode

```mcfunction
/gamemode <mode> <player>
```

---

# Inventory Commands

## Give Items

```mcfunction
/give <player> <item> <amount>
```

Example:

```mcfunction
/give Steve diamond 64
```

## Clear Inventory

```mcfunction
/clear <player>
```

## Clear Specific Item

```mcfunction
/clear <player> <item>
```

Example:

```mcfunction
/clear Steve dirt
```

## Replace Item In Hand

```mcfunction
/item replace entity <player> weapon.mainhand with <item>
```

Example:

```mcfunction
/item replace entity @p weapon.mainhand with diamond_sword
```

---

# Experience Commands

## Give XP Points

```mcfunction
/xp add <player> <amount>
```

Example:

```mcfunction
/xp add @p 100
```

## Give XP Levels

```mcfunction
/xp add <player> <amount> levels
```

Example:

```mcfunction
/xp add @p 10 levels
```

## Remove XP

```mcfunction
/xp add <player> -<amount>
```

---

# Effect Commands

## Give Effect

```mcfunction
/effect give <player> <effect> <duration> <amplifier>
```

Example:

```mcfunction
/effect give @p speed 60 5
```

## Remove All Effects

```mcfunction
/effect clear <player>
```

## Remove Specific Effect

```mcfunction
/effect clear <player> <effect>
```

Examples:

```mcfunction
/effect clear @p speed
```

---

# Player Movement Commands

## Set Spawn Point

```mcfunction
/spawnpoint
```

## Set Specific Spawn Location

```mcfunction
/spawnpoint <player> <x> <y> <z>
```

## Ride Entities

```mcfunction
/ride <player> mount <entity>
```

## Dismount

```mcfunction
/ride <player> dismount
```

---

# Player Information Commands

## Show Player List

```mcfunction
/list
```

## Show Player Position

```mcfunction
/data get entity <player> Pos
```

## Show Player Data

```mcfunction
/data get entity <player>
```

---

# Player Tags

## Add Tag

```mcfunction
/tag <player> add <tag>
```

Example:

```mcfunction
/tag Steve add builder
```

## Remove Tag

```mcfunction
/tag <player> remove <tag>
```

## List Tags

```mcfunction
/tag <player> list
```

---

# Player Abilities

## Give Operator Permission

```mcfunction
/op <player>
```

## Remove Operator Permission

```mcfunction
/deop <player>
```

## Change Player Permissions

Use server permission settings.

---

# Messaging Commands

## Send Message

```mcfunction
/msg <player> <message>
```

Example:

```mcfunction
/msg Steve Hello!
```

## Reply To Last Message

```mcfunction
/r <message>
```

## Broadcast Message

```mcfunction
/say <message>
```

Example:

```mcfunction
/say Welcome to the server!
```

## Tellraw Messages

```mcfunction
/tellraw <player> <json>
```

Example:

```mcfunction
/tellraw @a {"text":"Welcome!"}
```

---

# Player Target Selectors

## Nearest Player

```mcfunction
@p
```

## All Players

```mcfunction
@a
```

## Random Player

```mcfunction
@r
```

## All Entities

```mcfunction
@e
```

## Yourself

```mcfunction
@s
```

---

# Player Selector Examples

## Target Players Within Distance

```mcfunction
@a[distance=..10]
```

## Target Specific Player Name

```mcfunction
@a[name=Steve]
```

## Target Players In A Team

```mcfunction
@a[team=Red]
```

## Target Players At Coordinates

```mcfunction
@a[x=100,y=64,z=100]
```

---

# Player Utility Commands

## Kill Yourself

```mcfunction
/kill
```

## Kill Another Player

```mcfunction
/kill <player>
```

## Change Weather For Player

```mcfunction
/weather clear
```

## Enable Keep Inventory

```mcfunction
/gamerule keepInventory true
```

---

# Player Tips

- Use selectors like `@p`, `@a`, and `@s` to target players quickly.
- Combine commands with command blocks for custom systems.
- Use tags to create custom player groups.
- Always test powerful commands before using them on servers.

---

More player commands and advanced player systems will be added over time.
