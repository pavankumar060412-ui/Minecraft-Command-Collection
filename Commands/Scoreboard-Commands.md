# Minecraft Scoreboard Commands

A collection of commands used to create, manage, and control score systems, statistics, currencies, and custom game mechanics.

# Creating Scoreboards

## Create A Scoreboard Objective

```mcfunction
/scoreboard objectives add <name> <criteria>
```

Example:

```mcfunction
/scoreboard objectives add kills minecraft.killed:minecraft.zombie
```

---

# Display Scoreboards

## Show Scoreboard On Sidebar

```mcfunction
/scoreboard objectives setdisplay sidebar <objective>
```

Example:

```mcfunction
/scoreboard objectives setdisplay sidebar kills
```

## Show Scoreboard Above Player Name

```mcfunction
/scoreboard objectives setdisplay belowName <objective>
```

## Show Scoreboard In Player List

```mcfunction
/scoreboard objectives setdisplay list <objective>
```

---

# Managing Objectives

## List Scoreboards

```mcfunction
/scoreboard objectives list
```

## Remove Objective

```mcfunction
/scoreboard objectives remove <objective>
```

## Rename Objective

Create a new objective and remove the old one.

---

# Player Scores

## Add Score

```mcfunction
/scoreboard players add <player> <objective> <amount>
```

Example:

```mcfunction
/scoreboard players add @p points 10
```

## Remove Score

```mcfunction
/scoreboard players remove <player> <objective> <amount>
```

## Set Score

```mcfunction
/scoreboard players set <player> <objective> <amount>
```

Example:

```mcfunction
/scoreboard players set @p level 1
```

## Reset Score

```mcfunction
/scoreboard players reset <player>
```

---

# Scoreboard Criteria

## Dummy Objective

Used for custom systems.

```mcfunction
/scoreboard objectives add points dummy
```

## Player Kills

```text
playerKillCount
```

## Mob Kills

```text
totalKillCount
```

## Death Count

```text
deathCount
```

## Health Display

```text
health
```

## Mining Statistics

Examples:

```text
minecraft.mined:minecraft.stone
```

```text
minecraft.mined:minecraft.diamond_ore
```

## Item Used Statistics

Example:

```text
minecraft.used:minecraft.diamond_sword
```

---

# Useful Scoreboard Systems

## Create Money System

Create:

```mcfunction
/scoreboard objectives add money dummy Money
```

Give money:

```mcfunction
/scoreboard players add @p money 100
```

Remove money:

```mcfunction
/scoreboard players remove @p money 50
```

---

# Kill Counter

## Create Kill Counter

```mcfunction
/scoreboard objectives add kills playerKillCount
```

Display:

```mcfunction
/scoreboard objectives setdisplay sidebar kills
```

---

# Death Counter

Create:

```mcfunction
/scoreboard objectives add deaths deathCount
```

Display:

```mcfunction
/scoreboard objectives setdisplay sidebar deaths
```

---

# Health Display

Create:

```mcfunction
/scoreboard objectives add health health
```

Display:

```mcfunction
/scoreboard objectives setdisplay belowName health
```

---

# Team Score Systems

## Add Team

```mcfunction
/team add <team>
```

Example:

```mcfunction
/team add Red
```

## Join Team

```mcfunction
/team join <team> <player>
```

Example:

```mcfunction
/team join Red Steve
```

## Remove Team

```mcfunction
/team remove <team>
```

---

# Advanced Scoreboard Commands

## Compare Scores

```mcfunction
/execute if score <player> <objective> matches <value> run <command>
```

Example:

```mcfunction
/execute if score @p points matches 100 run say Winner!
```

## Copy Scores

```mcfunction
/scoreboard players operation <player> <objective> = <player> <objective>
```

## Add Scores Together

```mcfunction
/scoreboard players operation <player> <objective> += <player> <objective>
```

## Subtract Scores

```mcfunction
/scoreboard players operation <player> <objective> -= <player> <objective>
```

## Multiply Scores

```mcfunction
/scoreboard players operation <player> <objective> *= <player> <objective>
```

## Divide Scores

```mcfunction
/scoreboard players operation <player> <objective> /= <player> <objective>
```

---

# Minigame Examples

## Create Points System

```mcfunction
/scoreboard objectives add points dummy Points
```

Add points:

```mcfunction
/scoreboard players add @p points 1
```

## Create Timer

Create:

```mcfunction
/scoreboard objectives add timer dummy Timer
```

Add time:

```mcfunction
/scoreboard players add @a timer 1
```

---

# RPG Systems

## Create Level System

```mcfunction
/scoreboard objectives add level dummy Level
```

Increase Level:

```mcfunction
/scoreboard players add @p level 1
```

## Create Experience System

```mcfunction
/scoreboard objectives add xp dummy XP
```

---

# Scoreboard Tips

- Use dummy objectives for custom systems.
- Combine scoreboards with command blocks.
- Use `/execute if score` for logic systems.
- Scoreboards can create RPGs, shops, currencies, and minigames.

---

More advanced scoreboard systems and examples will be added over time.
