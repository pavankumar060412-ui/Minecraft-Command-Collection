# Minecraft Data Commands

A collection of commands used to read, modify, and manage Minecraft data stored inside entities, blocks, and storage systems.

# What Is The Data Command?

The `/data` command allows you to view and edit Minecraft's internal data (NBT data).

It is mainly used for:
- Custom mobs
- Custom items
- Advanced command systems
- Map making
- Automation

---

# Data Get Commands

## Get Entity Data

```mcfunction
/data get entity <entity>
```

Example:

```mcfunction
/data get entity @p
```

## Get Specific Entity Data

```mcfunction
/data get entity <entity> <path>
```

Example:

```mcfunction
/data get entity @p Pos
```

## Get Block Data

```mcfunction
/data get block <x> <y> <z>
```

Example:

```mcfunction
/data get block ~ ~ ~
```

## Get Storage Data

```mcfunction
/data get storage <namespace> <path>
```

---

# Data Merge Commands

## Modify Entity Data

```mcfunction
/data merge entity <entity> <nbt>
```

Example:

```mcfunction
/data merge entity @e[type=zombie,limit=1] {NoAI:1b}
```

## Modify Block Data

```mcfunction
/data merge block <x> <y> <z> <nbt>
```

## Modify Storage Data

```mcfunction
/data merge storage <namespace> <nbt>
```

---

# Data Modify Commands

## Set Data Value

```mcfunction
/data modify <target> set value <value>
```

Example:

```mcfunction
/data modify storage test value set value 100
```

## Copy Data

```mcfunction
/data modify <target> set from <source>
```

Example:

```mcfunction
/data modify entity @p Health set from entity @e[type=zombie,limit=1] Health
```

## Append Data

```mcfunction
/data modify <target> append value <value>
```

## Insert Data

```mcfunction
/data modify <target> insert <index> value <value>
```

---

# Entity Data Examples

## Remove Mob AI

```mcfunction
/data merge entity @e[type=zombie,limit=1] {NoAI:1b}
```

## Enable Mob AI

```mcfunction
/data merge entity @e[type=zombie,limit=1] {NoAI:0b}
```

## Make Entity Silent

```mcfunction
/data merge entity @e[type=zombie,limit=1] {Silent:1b}
```

## Make Entity Invulnerable

```mcfunction
/data merge entity @e[type=zombie,limit=1] {Invulnerable:1b}
```

## Make Entity Invisible

```mcfunction
/data merge entity @e[type=armor_stand,limit=1] {Invisible:1b}
```

---

# Custom Mob Examples

## Custom Name

```mcfunction
/data merge entity @e[type=zombie,limit=1] {CustomName:'{"text":"Boss Zombie"}'}
```

## Baby Zombie

```mcfunction
/data merge entity @e[type=zombie,limit=1] {IsBaby:1b}
```

## Giant Custom Health

```mcfunction
/data merge entity @e[type=zombie,limit=1] {Health:100}
```

---

# Item Data

## View Item Data

```mcfunction
/data get entity @p SelectedItem
```

## Custom Item Name

Example:

```mcfunction
/give @p diamond_sword{display:{Name:'{"text":"Legendary Sword"}'}}
```

## Custom Lore

```mcfunction
/give @p diamond_sword{display:{Lore:['{"text":"A powerful weapon"}']}}
```

---

# Custom Armor Stand Examples

## Invisible Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Invisible:1b}
```

## Small Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Small:1b}
```

## No Gravity Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {NoGravity:1b}
```

## Marker Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Marker:1b}
```

---

# Storage Data

## Create Storage Data

```mcfunction
/data merge storage mydata example 1
```

## Read Storage Data

```mcfunction
/data get storage mydata
```

Storage is useful for:
- Saving values
- Custom systems
- Advanced maps

---

# Block Data

## View Block Data

```mcfunction
/data get block <x> <y> <z>
```

## Modify Container Data

Example:

```mcfunction
/data get block ~ ~ ~ Items
```

---

# Advanced Uses

## Custom Bosses

Combine:
- `/summon`
- `/data`
- `/effect`
- `/attribute`

to create custom bosses.

## Custom Items

Combine:
- `/give`
- NBT data
- Enchantments
- Lore

to create unique items.

## Advanced Maps

Use:
- Storage
- Functions
- Scoreboards
- Execute commands

to create complex systems.

---

# Data Command Tips

- Always test NBT commands in a backup world.
- Incorrect NBT data can cause commands to fail.
- Combine `/data` with `/execute` for advanced creations.
- NBT allows almost unlimited customization.

---

More advanced NBT examples and custom creations will be added over time.
