# Minecraft Execute Commands

A complete guide to the `/execute` command, one of Minecraft's most powerful commands used for advanced systems, automation, maps, and command creations.

# What Is Execute?

The `/execute` command allows another command to run under specific conditions, locations, entities, or situations.

Basic format:

```mcfunction
/execute <subcommand> run <command>
```

Example:

```mcfunction
/execute as @p run say Hello
```

---

# Execute As

Runs a command as another entity.

## Run As Nearest Player

```mcfunction
/execute as @p run <command>
```

Example:

```mcfunction
/execute as @p run say I am the player
```

## Run As All Players

```mcfunction
/execute as @a run <command>
```

## Run As A Mob

```mcfunction
/execute as @e[type=zombie] run <command>
```

---

# Execute At

Runs a command from an entity's location.

## Execute At Player

```mcfunction
/execute at @p run <command>
```

Example:

```mcfunction
/execute at @p run summon lightning_bolt
```

## Execute At Mob

```mcfunction
/execute at @e[type=creeper] run <command>
```

---

# Execute As And At Together

Runs a command as an entity at its location.

Example:

```mcfunction
/execute as @e[type=zombie] at @s run say Zombie
```

Useful for:
- Mob systems
- Custom bosses
- Entity detection

---

# Execute If

Runs a command only if a condition is true.

Basic format:

```mcfunction
/execute if <condition> run <command>
```

---

# Execute If Entity

Checks if an entity exists.

Example:

```mcfunction
/execute if entity @p run say Player found
```

## Detect Nearby Players

```mcfunction
/execute if entity @a[distance=..5] run say Someone is nearby
```

---

# Execute Unless

Runs a command if something is NOT true.

Basic format:

```mcfunction
/execute unless <condition> run <command>
```

Example:

```mcfunction
/execute unless entity @p run say No players online
```

---

# Execute If Block

Checks if a block exists at a location.

Example:

```mcfunction
/execute if block ~ ~-1 ~ diamond_block run say Standing on diamond
```

---

# Execute If Blocks

Compares two areas.

Format:

```mcfunction
/execute if blocks <start> <end> <destination> all
```

---

# Execute If Score

Checks scoreboard values.

Format:

```mcfunction
/execute if score <player> <objective> matches <value> run <command>
```

Example:

```mcfunction
/execute if score @p points matches 10 run say Level complete
```

---

# Execute Unless Score

Runs when a score does not match.

Example:

```mcfunction
/execute unless score @p points matches 10 run say Not enough points
```

---

# Execute Positioned

Changes command location.

Example:

```mcfunction
/execute positioned 100 64 100 run summon zombie
```

---

# Execute Positioned As Entity

Runs at another entity's position.

Example:

```mcfunction
/execute at @e[type=creeper] run summon tnt
```

---

# Execute Rotated

Changes command rotation.

Example:

```mcfunction
/execute rotated ~ ~ run <command>
```

---

# Execute Facing

Makes a command face a direction.

Example:

```mcfunction
/execute facing entity @p eyes run particle flame
```

---

# Execute Store

Stores command results into data.

## Store Scoreboard Value

Example:

```mcfunction
/execute store result score @p points run data get entity @p Health
```

## Store Entity Data

```mcfunction
/execute store result entity <target> <path> run <command>
```

---

# Execute Examples

## Lightning When Player Walks

```mcfunction
/execute at @a run summon lightning_bolt
```

## TNT Around Creepers

```mcfunction
/execute at @e[type=creeper] run summon tnt
```

## Detect Diamond Block

```mcfunction
/execute if block ~ ~-1 ~ diamond_block run say Diamond floor!
```

## Give Effect Near Area

```mcfunction
/execute as @a[distance=..10] run effect give @s speed 5 2
```

---

# Advanced Execute Systems

## Custom Boss Detection

```mcfunction
/execute if entity @e[tag=boss] run say Boss Alive
```

## Automatic Door System

```mcfunction
/execute if entity @p[distance=..3] run setblock ~ ~ ~ air
```

## Mob Ability System

```mcfunction
/execute as @e[type=zombie,tag=boss] at @s run effect give @a strength 5 2
```

---

# Execute Tips

- Combine `as` and `at` for advanced entity systems.
- Use `if` and `unless` for logic.
- Use scoreboards with execute for games.
- Execute is the foundation of advanced command creations.

---

More advanced execute systems and examples will be added over time.
