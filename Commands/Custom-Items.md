# Minecraft Custom Items

A collection of commands used to create custom items with names, lore, enchantments, and special properties.

# What Are Custom Items?

Custom items are Minecraft items modified using commands or NBT data.

They are useful for:
- Adventure maps
- RPG servers
- Custom weapons
- Special rewards
- Minigames

---

# Custom Item Names

## Rename An Item

```mcfunction
/give @p diamond_sword{display:{Name:'{"text":"Legendary Sword"}'}}
```

---

# Custom Item Lore

## Add Description Text

```mcfunction
/give @p diamond_sword{display:{Lore:['{"text":"A sword of legends"}']}}
```

---

# Multiple Lore Lines

```mcfunction
/give @p diamond_sword{display:{Lore:['{"text":"Legendary Weapon"}','{"text":"Created by the gods"}']}}
```

---

# Custom Enchanted Items

## Sharpness Sword

```mcfunction
/give @p diamond_sword{Enchantments:[{id:"minecraft:sharpness",lvl:5}]}
```

---

## Multiple Enchantments

```mcfunction
/give @p diamond_sword{Enchantments:[{id:"minecraft:sharpness",lvl:5},{id:"minecraft:fire_aspect",lvl:2}]}
```

---

# Unbreakable Items

```mcfunction
/give @p diamond_pickaxe{Unbreakable:1b}
```

---

# Custom Model Data

Used for resource packs.

```mcfunction
/give @p stick{CustomModelData:1}
```

---

# Custom Weapons

## Fire Sword

```mcfunction
/give @p diamond_sword{display:{Name:'{"text":"Fire Sword"}'},Enchantments:[{id:"minecraft:fire_aspect",lvl:10}]}
```

---

## God Sword

```mcfunction
/give @p netherite_sword{Enchantments:[{id:"minecraft:sharpness",lvl:255},{id:"minecraft:unbreaking",lvl:255},{id:"minecraft:looting",lvl:255}]}
```

---

# Custom Armor

## Dragon Helmet

```mcfunction
/give @p netherite_helmet{display:{Name:'{"text":"Dragon Helmet"}'}}
```

---

## Powerful Chestplate

```mcfunction
/give @p netherite_chestplate{Enchantments:[{id:"minecraft:protection",lvl:10}]}
```

---

# Custom Tools

## Fast Pickaxe

```mcfunction
/give @p diamond_pickaxe{Enchantments:[{id:"minecraft:efficiency",lvl:10}]}
```

---

## Fortune Tool

```mcfunction
/give @p diamond_pickaxe{Enchantments:[{id:"minecraft:fortune",lvl:5}]}
```

---

# Custom Food

## Named Apple

```mcfunction
/give @p golden_apple{display:{Name:'{"text":"Royal Apple"}'}}
```

---

# Custom Potions

## Speed Potion

```mcfunction
/give @p potion{Potion:"minecraft:swiftness"}
```

---

## Strength Potion

```mcfunction
/give @p potion{Potion:"minecraft:strength"}
```

---

# Custom Special Items

## Knockback Stick

```mcfunction
/give @p stick{Enchantments:[{id:"minecraft:knockback",lvl:10}]}
```

---

## Invisible Item Display

```mcfunction
/summon item_display ~ ~ ~ {item:{id:"minecraft:diamond",count:1}}
```

---

# Custom Item Systems

Combine custom items with:

- Tags
- Scoreboards
- Execute commands
- Advancements
- Functions

to create:

- RPG weapons
- Quest rewards
- Boss drops
- Special abilities

---

# Custom Item Tips

- Use names and lore to make items unique.
- Combine enchantments for powerful gear.
- Use resource packs with CustomModelData.
- Test commands before using them in servers.

---

More advanced custom item creations will be added over time.
