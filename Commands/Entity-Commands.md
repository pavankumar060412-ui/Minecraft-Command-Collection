# Minecraft Entity Commands

A collection of commands used to create, control, modify, and manage entities in Minecraft.

# Summon Commands

## Summon Any Entity

```mcfunction
/summon <entity>
```

Example:

```mcfunction
/summon minecraft:zombie
```

## Summon Entity At Coordinates

```mcfunction
/summon <entity> <x> <y> <z>
```

Example:

```mcfunction
/summon minecraft:creeper 100 64 100
```

## Summon Entity With Rotation

```mcfunction
/summon <entity> <x> <y> <z> <rotation>
```

---

# Entity Target Selectors

## All Entities

```mcfunction
@e
```

## All Mobs

```mcfunction
@e[type=!player]
```

## Specific Entity Type

```mcfunction
@e[type=minecraft:zombie]
```

Example:

```mcfunction
/kill @e[type=minecraft:creeper]
```

## Entities Near A Location

```mcfunction
@e[distance=..10]
```

## Entities With Names

```mcfunction
@e[name=Bob]
```

## Entities With Tags

```mcfunction
@e[tag=test]
```

---

# Entity Management

## Kill All Entities

```mcfunction
/kill @e
```

## Remove All Dropped Items

```mcfunction
/kill @e[type=item]
```

## Remove All Mobs

```mcfunction
/kill @e[type=!player]
```

## Remove Specific Mob

```mcfunction
/kill @e[type=minecraft:zombie]
```

---

# Entity Data Commands

## View Entity Data

```mcfunction
/data get entity <entity>
```

Example:

```mcfunction
/data get entity @e[type=minecraft:zombie,limit=1]
```

## Modify Entity Data

```mcfunction
/data modify entity <entity> <path>
```

Example:

```mcfunction
/data modify entity @e[type=minecraft:zombie,limit=1] Health
```

---

# Entity Tags

## Add Tag To Entity

```mcfunction
/tag <entity> add <tag>
```

Example:

```mcfunction
/tag @e[type=zombie,limit=1] add boss
```

## Remove Tag

```mcfunction
/tag <entity> remove <tag>
```

## List Tags

```mcfunction
/tag <entity> list
```

---

# Entity Movement

## Teleport Entity

```mcfunction
/tp <entity> <x> <y> <z>
```

Example:

```mcfunction
/tp @e[type=zombie] 0 100 0
```

## Move Entity To Player

```mcfunction
/tp <entity> <player>
```

---

# Ride Commands

## Make Entity Ride Another Entity

```mcfunction
/ride <entity> mount <vehicle>
```

Example:

```mcfunction
/ride @p mount @e[type=horse,limit=1]
```

## Remove Rider

```mcfunction
/ride <entity> dismount
```

---

# Entity Effects

## Give Effect To Entity

```mcfunction
/effect give <entity> <effect> <time> <level>
```

Example:

```mcfunction
/effect give @e[type=zombie] speed 100 5
```

## Remove Effects

```mcfunction
/effect clear <entity>
```

---

# Mob Control

## Freeze Mobs

```mcfunction
/effect give @e[type=!player] slowness 99999 255
```

## Make Mobs Stronger

```mcfunction
/effect give @e[type=zombie] strength 99999 5
```

## Remove Mob AI

```mcfunction
/data merge entity <entity> {NoAI:1b}
```

Example:

```mcfunction
/data merge entity @e[type=zombie,limit=1] {NoAI:1b}
```

## Enable Mob AI

```mcfunction
/data merge entity <entity> {NoAI:0b}
```

---

# Custom Entity Examples

## Invisible Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Invisible:1b}
```

## Small Slime

```mcfunction
/summon slime ~ ~ ~ {Size:1}
```

## Giant Zombie

```mcfunction
/summon zombie ~ ~ ~ {IsBaby:0}
```

## Custom Named Entity

```mcfunction
/summon zombie ~ ~ ~ {CustomName:'{"text":"Boss Zombie"}'}
```

---

# Entity Equipment

## Give Mob Item

```mcfunction
/item replace entity <entity> weapon.mainhand with <item>
```

Example:

```mcfunction
/item replace entity @e[type=zombie,limit=1] weapon.mainhand with diamond_sword
```

---

# Entity Attributes

## View Attributes

```mcfunction
/attribute <target> <attribute> get
```

## Modify Attributes

```mcfunction
/attribute <target> <attribute> base set <value>
```

Examples:

```mcfunction
/attribute @p minecraft:generic.max_health base set 40
```

---

# Useful Entity Commands

## Find Nearest Entity

```mcfunction
/execute as @e[type=zombie,limit=1] run say Found
```

## Execute Command As Entity

```mcfunction
/execute as <entity> run <command>
```

## Execute At Entity Location

```mcfunction
/execute at <entity> run <command>
```

---

# Entity Tips

- Use selectors to control specific groups of entities.
- Tags are useful for custom mobs and systems.
- Combine `/execute` with entities for advanced creations.
- Always test entity commands in a backup world.

---

More advanced entity commands, custom mobs, and automation systems will be added over time.
