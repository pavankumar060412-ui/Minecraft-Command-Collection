# Minecraft Tag Commands

A collection of commands used to create, manage, and use tags for players and entities in Minecraft.

# What Are Tags?

Tags are custom labels that can be added to players and entities.

They are useful for:
- Custom mobs
- Command systems
- Minigames
- RPG systems
- Advanced automation

Basic format:

```mcfunction
/tag <target> <action> <tag>
```

---

# Adding Tags

## Add A Tag To A Player

```mcfunction
/tag <player> add <tag>
```

Example:

```mcfunction
/tag Steve add warrior
```

## Add A Tag To An Entity

```mcfunction
/tag <entity> add <tag>
```

Example:

```mcfunction
/tag @e[type=zombie,limit=1] add boss
```

---

# Removing Tags

## Remove A Tag

```mcfunction
/tag <target> remove <tag>
```

Example:

```mcfunction
/tag Steve remove warrior
```

## Remove Entity Tag

```mcfunction
/tag @e[tag=boss] remove boss
```

---

# Listing Tags

## View Tags On Target

```mcfunction
/tag <target> list
```

Example:

```mcfunction
/tag @p list
```

---

# Using Tags With Selectors

Tags can be used inside selectors.

## Find Entities With A Tag

```mcfunction
@e[tag=<tag>]
```

Example:

```mcfunction
@e[tag=boss]
```

## Find Players With A Tag

```mcfunction
@a[tag=admin]
```

---

# Execute With Tags

## Run Command On Tagged Entities

```mcfunction
/execute as @e[tag=boss] run <command>
```

Example:

```mcfunction
/execute as @e[tag=boss] run say Boss detected
```

## Run Command At Tagged Entity

```mcfunction
/execute at @e[tag=boss] run <command>
```

Example:

```mcfunction
/execute at @e[tag=boss] run summon lightning_bolt
```

---

# Custom Mob Systems

## Create A Boss Tag

Add tag:

```mcfunction
/tag @e[type=zombie,limit=1] add boss
```

Detect boss:

```mcfunction
/execute if entity @e[tag=boss] run say Boss is alive
```

---

# Custom Classes

## Warrior Player

```mcfunction
/tag @p add warrior
```

## Mage Player

```mcfunction
/tag @p add mage
```

## Archer Player

```mcfunction
/tag @p add archer
```

Detect class:

```mcfunction
/execute as @a[tag=warrior] run effect give @s strength 5 1
```

---

# Minigame Systems

## Add Player To Team Role

```mcfunction
/tag @p add red_team
```

## Detect Team Players

```mcfunction
@a[tag=red_team]
```

## Give Team Ability

```mcfunction
/effect give @a[tag=red_team] strength 10 1
```

---

# Automatic Systems

## Detect Tagged Players

```mcfunction
/execute if entity @a[tag=vip] run say VIP Online
```

## Teleport Tagged Players

```mcfunction
/tp @a[tag=teleport] 0 100 0
```

## Remove Tagged Entities

```mcfunction
/kill @e[tag=remove]
```

---

# Advanced Tag Examples

## Create Custom Boss

Summon:

```mcfunction
/summon zombie ~ ~ ~
```

Add tag:

```mcfunction
/tag @e[type=zombie,limit=1] add boss
```

Give abilities:

```mcfunction
/effect give @e[tag=boss] strength 99999 5
```

---

# Tag Tips

- Tags do not disappear after leaving the world.
- Tags are stored on entities.
- Combine tags with `/execute` for advanced systems.
- Tags are faster and cleaner than checking names.
- Use unique tag names to avoid conflicts.

---

More advanced tag systems and examples will be added over time.
