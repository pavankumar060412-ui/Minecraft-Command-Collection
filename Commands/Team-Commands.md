# Minecraft Team Commands

A collection of commands used to create, manage, and customize player teams in Minecraft.

# What Are Teams?

Teams allow players to be grouped together with:
- Custom colors
- Names
- Prefixes
- Suffixes
- Friendly fire settings
- Visibility options

Teams are useful for:
- Multiplayer servers
- Minigames
- PvP systems
- Roleplay worlds

---

# Creating Teams

## Create A Team

```mcfunction
/team add <team_name>
```

Example:

```mcfunction
/team add Red
```

## Create Team With Display Name

```mcfunction
/team add <team_name> <display_name>
```

Example:

```mcfunction
/team add Blue "Blue Warriors"
```

---

# Managing Teams

## List Teams

```mcfunction
/team list
```

## Remove A Team

```mcfunction
/team remove <team_name>
```

Example:

```mcfunction
/team remove Red
```

## Get Team Information

```mcfunction
/team list <team_name>
```

---

# Adding Players To Teams

## Add Player To Team

```mcfunction
/team join <team_name> <player>
```

Example:

```mcfunction
/team join Red Steve
```

## Add Multiple Players

```mcfunction
/team join Red @a
```

## Remove Player From Team

```mcfunction
/team leave <player>
```

Example:

```mcfunction
/team leave Steve
```

---

# Team Colors

## Set Team Color

```mcfunction
/team modify <team> color <color>
```

Examples:

```mcfunction
/team modify Red color red
```

```mcfunction
/team modify Blue color blue
```

Available colors:

```
black
dark_blue
dark_green
dark_aqua
dark_red
dark_purple
gold
gray
dark_gray
blue
green
aqua
red
light_purple
yellow
white
```

---

# Team Prefixes And Suffixes

## Add Prefix

```mcfunction
/team modify <team> prefix <text>
```

Example:

```mcfunction
/team modify Red prefix "[RED] "
```

## Add Suffix

```mcfunction
/team modify <team> suffix " <text>"
```

Example:

```mcfunction
/team modify Red suffix " Warrior"
```

---

# Team Visibility

## Control Name Tag Visibility

```mcfunction
/team modify <team> nametagVisibility <option>
```

Options:

```
always
never
hideForOtherTeams
hideForOwnTeam
```

Example:

```mcfunction
/team modify Red nametagVisibility never
```

---

# Team Collision

## Enable Team Collision

```mcfunction
/team modify <team> collisionRule always
```

## Disable Team Collision

```mcfunction
/team modify <team> collisionRule never
```

Options:

```
always
never
pushOtherTeams
pushOwnTeam
```

---

# Friendly Fire

## Allow Team Members To Damage Each Other

```mcfunction
/team modify <team> friendlyFire true
```

## Disable Friendly Fire

```mcfunction
/team modify <team> friendlyFire false
```

---

# Team-Based Minigames

## Create Red Team

```mcfunction
/team add Red
/team modify Red color red
```

## Create Blue Team

```mcfunction
/team add Blue
/team modify Blue color blue
```

## Add Players

```mcfunction
/team join Red Player1
```

```mcfunction
/team join Blue Player2
```

---

# Detect Team Players

## Target A Specific Team

```mcfunction
@a[team=Red]
```

Example:

```mcfunction
/effect give @a[team=Red] strength 10 1
```

---

# Team Scoreboard Systems

Create team score:

```mcfunction
/scoreboard objectives add TeamScore dummy
```

Add points:

```mcfunction
/scoreboard players add @a[team=Red] TeamScore 1
```

---

# Team Commands With Execute

## Run Command For Team

```mcfunction
/execute as @a[team=Red] run <command>
```

Example:

```mcfunction
/execute as @a[team=Red] run effect give @s speed 10 1
```

---

# Useful Team Setups

## Red Vs Blue PvP

Red team:

```mcfunction
/team add Red
/team modify Red color red
```

Blue team:

```mcfunction
/team add Blue
/team modify Blue color blue
```

Disable friendly fire:

```mcfunction
/team modify Red friendlyFire false
/team modify Blue friendlyFire false
```

---

# Team Tips

- Combine teams with scoreboards for advanced games.
- Use colors and prefixes to identify players.
- Teams are useful for PvP and adventure maps.
- Use selectors like `@a[team=name]` for commands.

---

More advanced team systems and multiplayer setups will be added over time.
