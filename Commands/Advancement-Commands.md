# Minecraft Advancement Commands

A collection of commands used to manage achievements, progression systems, and custom challenges in Minecraft.

# What Are Advancements?

Advancements are Minecraft's built-in achievement system.

They can be used for:
- Custom challenges
- Adventure maps
- Progress tracking
- Reward systems
- RPG mechanics

---

# Advancement Command Basics

## Grant Advancement

```mcfunction
/advancement grant <player> <action>
```

Example:

```mcfunction
/advancement grant @p everything
```

---

# Grant Advancement Options

## Grant Everything

```mcfunction
/advancement grant @p everything
```

Gives all advancements.

## Grant Only One Advancement

```mcfunction
/advancement grant @p only <advancement>
```

Example:

```mcfunction
/advancement grant @p only minecraft:story/mine_stone
```

## Grant From A Point

```mcfunction
/advancement grant @p from <advancement>
```

Gives an advancement and everything below it.

## Grant Through

```mcfunction
/advancement grant @p through <advancement>
```

Gives all requirements up to that advancement.

---

# Removing Advancements

## Remove All Advancements

```mcfunction
/advancement revoke @p everything
```

## Remove Specific Advancement

```mcfunction
/advancement revoke @p only <advancement>
```

Example:

```mcfunction
/advancement revoke @p only minecraft:story/mine_stone
```

## Remove Advancement Tree

```mcfunction
/advancement revoke @p from <advancement>
```

---

# Useful Advancement Examples

## Give Stone Age Advancement

```mcfunction
/advancement grant @p only minecraft:story/mine_stone
```

## Give Getting An Upgrade

```mcfunction
/advancement grant @p only minecraft:story/upgrade_tools
```

## Give Diamonds Advancement

```mcfunction
/advancement grant @p only minecraft:story/mine_diamond
```

## Give Nether Advancement

```mcfunction
/advancement grant @p only minecraft:nether/root
```

---

# Checking Advancements

## Check If Player Has Advancement

```mcfunction
/execute if entity @a[advancements={minecraft:story/mine_stone=true}] run say Completed
```

---

# Advancement Criteria

Advancements can be triggered by:

## Mining Blocks

Example:

```text
minecraft:mined
```

## Crafting Items

Example:

```text
minecraft:recipe_unlocked
```

## Killing Entities

Example:

```text
minecraft:killed
```

## Using Items

Example:

```text
minecraft:using_item
```

## Location

Example:

```text
minecraft:location
```

## Effects

Example:

```text
minecraft:effects_changed
```

---

# Custom Advancement Systems

## Reward Player After Achievement

Example:

```mcfunction
/advancement grant @p only minecraft:story/mine_stone
```

Then use a command block:

```mcfunction
/give @p diamond
```

---

# RPG Level System

Combine:

- Advancements
- Scoreboards
- Tags
- Commands

Example:

When player completes challenge:

```mcfunction
/scoreboard players add @p level 1
```

---

# Adventure Map Examples

## Secret Room Achievement

Create a trigger:

```text
secret_room_found
```

Reward:

```mcfunction
/give @p emerald 5
```

## Boss Defeat Achievement

Detect boss:

```mcfunction
/execute unless entity @e[tag=boss] run advancement grant @a only custom:boss_defeated
```

---

# Advancement Tips

- Advancements can replace complicated command detection systems.
- They work well with datapacks.
- Combine advancements with rewards for custom gameplay.
- Use unique names for custom advancements.

---

More custom advancement systems and datapack examples will be added over time.
