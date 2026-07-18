# Minecraft Command Tutorial

A complete beginner-to-advanced guide for using commands in Minecraft.

# What Are Commands?

Commands are special instructions that allow players to control the Minecraft world.

Commands can be used for:

- Building
- Administration
- Automation
- Adventure maps
- Custom systems

---

# Enabling Commands

Commands can be enabled by:

## Singleplayer

Enable:

```text
Allow Cheats: ON
```

---

## Multiplayer

You need:

```text
Operator (OP) Permission
```

---

# Command Format

Basic command structure:

```mcfunction
/command <target> <value>
```

Example:

```mcfunction
/give @p diamond 64
```

---

# Target Selectors

## Nearest Player

```mcfunction
@p
```

Targets the closest player.

---

## All Players

```mcfunction
@a
```

Targets every player.

---

## Random Player

```mcfunction
@r
```

Targets a random player.

---

## All Entities

```mcfunction
@e
```

Targets all entities.

---

## Command Executor

```mcfunction
@s
```

Targets the entity running the command.

---

# Basic Commands

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
/tp <player> <coordinates>
```

Example:

```mcfunction
/tp @p 100 64 100
```

---

## Change Gamemode

```mcfunction
/gamemode <mode>
```

Modes:

```text
survival
creative
adventure
spectator
```

---

## Kill Entities

```mcfunction
/kill <target>
```

Example:

```mcfunction
/kill @e[type=zombie]
```

---

## Weather Control

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

## Time Control

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

# Building Commands

## Fill Command

Used to fill areas.

```mcfunction
/fill <from> <to> <block>
```

Example:

```mcfunction
/fill ~ ~ ~ ~10 ~10 ~10 stone
```

---

## Clone Command

Copies builds.

```mcfunction
/clone <start> <end> <destination>
```

---

## Set Block

Places a block.

```mcfunction
/setblock <location> <block>
```

---

# Effects

Give effects:

```mcfunction
/effect give <player> <effect> <time> <level>
```

Example:

```mcfunction
/effect give @p speed 60 2
```

---

# Enchant Commands

Enchant held items:

```mcfunction
/enchant <player> <enchantment> <level>
```

Example:

```mcfunction
/enchant @p sharpness 5
```

---

# Experience Commands

Give XP:

```mcfunction
/xp add <player> <amount>
```

Example:

```mcfunction
/xp add @p 100 levels
```

---

# Summoning Entities

Summon mobs:

```mcfunction
/summon <entity>
```

Example:

```mcfunction
/summon zombie
```

---

# Command Blocks

Command blocks allow commands to run automatically.

Give command block:

```mcfunction
/give @p command_block
```

Types:

- Impulse
- Repeat
- Chain

---

# Execute Command

Execute allows advanced command systems.

Basic format:

```mcfunction
/execute as <target> run <command>
```

Example:

```mcfunction
/execute as @a run say Hello
```

---

# Scoreboards

Create scoreboard:

```mcfunction
/scoreboard objectives add <name> dummy
```

Add score:

```mcfunction
/scoreboard players add <player> <objective> <amount>
```

---

# Tags

Add a tag:

```mcfunction
/tag <player> add <tag>
```

Remove tag:

```mcfunction
/tag <player> remove <tag>
```

---

# Functions

Functions allow multiple commands to run together.

Run:

```mcfunction
/function <name>
```

---

# Command Tips

- Test commands in creative mode first.
- Use command blocks for automation.
- Learn execute for advanced systems.
- Use tags and scoreboards for custom maps.
- Keep command files organized.

---

# Advanced Command Ideas

Create:

- Custom bosses
- Minigames
- Teleport systems
- Custom items
- Adventure maps
- Automated machines

---

More command tutorials will be added over time.
