# Minecraft NBT Data Examples

A collection of examples using Minecraft NBT data for advanced commands, custom items, and custom entities.

# What Is NBT?

NBT (Named Binary Tag) is Minecraft's system for storing data.

NBT is used for:
- Custom items
- Custom mobs
- Entity settings
- Data storage
- Advanced commands

---

# Viewing NBT Data

## View Player Data

```mcfunction
/data get entity @p
```

## View Selected Item Data

```mcfunction
/data get entity @p SelectedItem
```

## View Entity Data

```mcfunction
/data get entity @e[type=zombie,limit=1]
```

---

# Custom Items

## Named Sword

```mcfunction
/give @p diamond_sword{display:{Name:'{"text":"Legendary Sword"}'}}
```

---

## Sword With Lore

```mcfunction
/give @p diamond_sword{display:{Name:'{"text":"Legendary Sword"}',Lore:['{"text":"A powerful weapon"}']}}
```

---

## Enchanted Sword

```mcfunction
/give @p diamond_sword{Enchantments:[{id:"minecraft:sharpness",lvl:5}]}
```

---

# Custom Armor

## Named Armor

```mcfunction
/give @p diamond_chestplate{display:{Name:'{"text":"Dragon Armor"}'}}
```

---

## Enchanted Armor

```mcfunction
/give @p diamond_helmet{Enchantments:[{id:"minecraft:protection",lvl:4}]}
```

---

# Entity NBT Examples

## No AI Mob

```mcfunction
/summon zombie ~ ~ ~ {NoAI:1b}
```

---

## Silent Mob

```mcfunction
/summon zombie ~ ~ ~ {Silent:1b}
```

---

## Invulnerable Mob

```mcfunction
/summon zombie ~ ~ ~ {Invulnerable:1b}
```

---

## Custom Name Mob

```mcfunction
/summon zombie ~ ~ ~ {CustomName:'{"text":"Boss Zombie"}'}
```

---

## Baby Zombie

```mcfunction
/summon zombie ~ ~ ~ {IsBaby:1b}
```

---

# Armor Stand NBT

## Invisible Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Invisible:1b}
```

---

## Small Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Small:1b}
```

---

## No Gravity Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {NoGravity:1b}
```

---

## Marker Armor Stand

```mcfunction
/summon armor_stand ~ ~ ~ {Marker:1b}
```

---

# Item NBT

## Custom Count

```mcfunction
/give @p diamond{Count:64}
```

---

## Unbreakable Item

```mcfunction
/give @p diamond_pickaxe{Unbreakable:1b}
```

---

## Custom Item Model

```mcfunction
/give @p stick{CustomModelData:1}
```

---

# Entity Attributes

## High Health Mob

```mcfunction
/summon zombie ~ ~ ~ {Attributes:[{Name:"minecraft:generic.max_health",Base:100}]}
```

---

## Fast Mob

```mcfunction
/summon zombie ~ ~ ~ {Attributes:[{Name:"minecraft:generic.movement_speed",Base:0.5}]}
```

---

# Data Modify Examples

## Change Entity Data

```mcfunction
/data merge entity @e[type=zombie,limit=1] {NoAI:1b}
```

---

## Change Storage Data

```mcfunction
/data merge storage example:data {level:10}
```

---

# Custom Boss Example

```mcfunction
/summon zombie ~ ~ ~ {CustomName:'{"text":"Ancient Boss"}',Health:200,Attributes:[{Name:"minecraft:generic.max_health",Base:200}],NoAI:0b}
```

---

# NBT Tips

- Always test NBT commands in a backup world.
- NBT changes can completely modify entities and items.
- Combine NBT with `/execute` for advanced systems.
- Modern Minecraft versions may change NBT formats.

---

More advanced NBT creations will be added over time.
