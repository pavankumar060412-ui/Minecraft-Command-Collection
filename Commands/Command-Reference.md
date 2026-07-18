# Minecraft Command Reference

A complete reference list of Minecraft commands and their uses.

# What Are Commands?

Commands are powerful tools used to control Minecraft worlds, players, entities, and systems.

Commands can be used for:
- Building
- Administration
- Automation
- Adventure maps
- Custom game modes

---

# Administration Commands

## Ban Player

```mcfunction
/ban <player>
```

## Ban IP Address

```mcfunction
/ban-ip <address>
```

## Unban Player

```mcfunction
/pardon <player>
```

## Kick Player

```mcfunction
/kick <player>
```

## Give Operator

```mcfunction
/op <player>
```

## Remove Operator

```mcfunction
/deop <player>
```

---

# World Commands

## Change Gamemode

```mcfunction
/gamemode <mode> <player>
```

Modes:

```text
survival
creative
adventure
spectator
```

---

## Change Difficulty

```mcfunction
/difficulty <level>
```

Levels:

```text
peaceful
easy
normal
hard
```

---

## Set Time

```mcfunction
/time set <value>
```

Examples:

```mcfunction
/time set day
```

```mcfunction
/time set night
```

---

## Weather

```mcfunction
/weather <type>
```

Types:

```text
clear
rain
thunder
```

---

# Player Commands

## Give Items

```mcfunction
/give <player> <item> <amount>
```

Example:

```mcfunction
/give @p diamond 64
```

---

## Teleport

```mcfunction
/tp <target> <location>
```

Example:

```mcfunction
/tp @p 100 64 100
```

---

## Kill

```mcfunction
/kill <target>
```

Example:

```mcfunction
/kill @e[type=zombie]
```

---

# Building Commands

## Fill Area

```mcfunction
/fill <from> <to> <block>
```

Example:

```mcfunction
/fill ~ ~ ~ ~10 ~10 ~10 stone
```

---

## Clone Area

```mcfunction
/clone <start> <end> <destination>
```

---

## Set Block

```mcfunction
/setblock <location> <block>
```

Example:

```mcfunction
/setblock ~ ~ ~ diamond_block
```

---

# Entity Commands

## Summon Entity

```mcfunction
/summon <entity>
```

Example:

```mcfunction
/summon zombie
```

---

## Effect Command

```mcfunction
/effect give <player> <effect> <time> <level>
```

Example:

```mcfunction
/effect give @p speed 60 2
```

---

# Advanced Commands

## Execute

```mcfunction
/execute <subcommand> run <command>
```

Example:

```mcfunction
/execute as @a run say Hello
```

---

## Data

```mcfunction
/data get entity <target>
```

Used for NBT data.

---

## Scoreboard

Create scoreboard:

```mcfunction
/scoreboard objectives add <name> dummy
```

Add points:

```mcfunction
/scoreboard players add <player> <objective> <amount>
```

---

## Tags

Add tag:

```mcfunction
/tag <target> add <tag>
```

Remove tag:

```mcfunction
/tag <target> remove <tag>
```

---

## Teams

Create team:

```mcfunction
/team add <team>
```

Join team:

```mcfunction
/team join <team> <player>
```

---

## Functions

Run function:

```mcfunction
/function <function>
```

---

## Schedule

Schedule function:

```mcfunction
/schedule function <function> <time>
```

---

## Loot

Give loot:

```mcfunction
/loot give <player> loot <table>
```

---

## Recipe

Unlock recipe:

```mcfunction
/recipe give <player> <recipe>
```

---

## Structure

Load structure:

```mcfunction
/structure load <name>
```

---

# Target Selectors

Nearest player:

```mcfunction
@p
```

All players:

```mcfunction
@a
```

Random player:

```mcfunction
@r
```

All entities:

```mcfunction
@e
```

Command executor:

```mcfunction
@s
```

---

# Command Block Commands

Give command block:

```mcfunction
/give @p command_block
```

Give repeating command block:

```mcfunction
/give @p repeating_command_block
```

Give chain command block:

```mcfunction
/give @p chain_command_block
```

---

# Common Utility Commands

## Say Message

```mcfunction
/say <message>
```

## Tell Player

```mcfunction
/tell <player> <message>
```

## Clear Inventory

```mcfunction
/clear <player>
```

## Experience

```mcfunction
/xp add <player> <amount>
```

---

# Command Tips

- Always test commands before using them in important worlds.
- Combine commands with functions for large systems.
- Use scoreboards for advanced logic.
- Use tags for custom entity systems.
- Use execute for advanced command creations.

---

# End Of Command Collection

This repository contains guides for:
- Basic commands
- Building systems
- Admin commands
- Advanced command systems
- Custom creations
- Automation

More Minecraft command updates can be added as new versions release.
