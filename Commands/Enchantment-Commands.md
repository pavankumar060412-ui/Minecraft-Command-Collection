# Minecraft Enchantment Commands

A collection of commands used to apply, manage, and create enchanted items in Minecraft.

# Basic Enchantment Commands

## Enchant Held Item

```mcfunction
/enchant <player> <enchantment> <level>
```

Example:

```mcfunction
/enchant @p sharpness 5
```

## Give An Enchanted Item

```mcfunction
/give <player> <item>{Enchantments:[{id:<enchantment>,lvl:<level>}]} <amount>
```

Example:

```mcfunction
/give @p diamond_sword{Enchantments:[{id:sharpness,lvl:5}]} 1
```

---

# Weapon Enchantments

## Sharpness

```text
sharpness
```

Increases melee damage.

Example:

```mcfunction
/enchant @p sharpness 5
```

## Smite

```text
smite
```

Extra damage against undead mobs.

## Bane Of Arthropods

```text
bane_of_arthropods
```

Extra damage against arthropods.

## Knockback

```text
knockback
```

Pushes enemies further away.

## Fire Aspect

```text
fire_aspect
```

Sets enemies on fire.

## Looting

```text
looting
```

Increases mob drops.

## Sweeping Edge

```text
sweeping
```

Increases sweep attack damage.

---

# Tool Enchantments

## Efficiency

```text
efficiency
```

Mines faster.

## Silk Touch

```text
silk_touch
```

Allows blocks to drop themselves.

## Fortune

```text
fortune
```

Increases block drops.

## Unbreaking

```text
unbreaking
```

Improves durability.

## Mending

```text
mending
```

Repairs items using XP.

---

# Armor Enchantments

## Protection

```text
protection
```

Reduces damage.

## Fire Protection

```text
fire_protection
```

Reduces fire damage.

## Blast Protection

```text
blast_protection
```

Reduces explosion damage.

## Projectile Protection

```text
projectile_protection
```

Reduces projectile damage.

## Feather Falling

```text
feather_falling
```

Reduces fall damage.

## Respiration

```text
respiration
```

Allows longer underwater breathing.

## Aqua Affinity

```text
aqua_affinity
```

Allows faster underwater mining.

## Thorns

```text
thorns
```

Damages attackers.

---

# Helmet Enchantments

## Turtle Helmet Effects

```text
respiration
```

## Aqua Mining

```text
aqua_affinity
```

---

# Leggings Enchantments

## Swift Sneak

```text
swift_sneak
```

Allows faster sneaking.

---

# Boots Enchantments

## Depth Strider

```text
depth_strider
```

Allows faster swimming.

## Frost Walker

```text
frost_walker
```

Creates ice while walking on water.

## Soul Speed

```text
soul_speed
```

Allows faster movement on soul blocks.

---

# Bow Enchantments

## Power

```text
power
```

Increases arrow damage.

## Punch

```text
punch
```

Increases arrow knockback.

## Flame

```text
flame
```

Shoots flaming arrows.

## Infinity

```text
infinity
```

Allows unlimited arrows.

## Mending

```text
mending
```

Repairs bow using XP.

---

# Crossbow Enchantments

## Multishot

```text
multishot
```

Shoots multiple arrows.

## Piercing

```text
piercing
```

Arrows pass through enemies.

## Quick Charge

```text
quick_charge
```

Loads faster.

---

# Trident Enchantments

## Loyalty

```text
loyalty
```

Returns the trident.

## Impaling

```text
impaling
```

Extra aquatic damage.

## Riptide

```text
riptide
```

Launches player with trident.

## Channeling

```text
channeling
```

Summons lightning during storms.

---

# Fishing Rod Enchantments

## Luck Of The Sea

```text
luck_of_the_sea
```

Better fishing loot.

## Lure

```text
lure
```

Catches fish faster.

---

# Mace Enchantments

## Density

```text
density
```

Increases smash damage.

## Breach

```text
breach
```

Reduces armor effectiveness.

## Wind Burst

```text
wind_burst
```

Launches player after smashing.

---

# Custom OP Enchantment Examples

## Sharpness 255 Sword

```mcfunction
/give @p diamond_sword{Enchantments:[{id:sharpness,lvl:255}]} 1
```

## Efficiency 255 Pickaxe

```mcfunction
/give @p diamond_pickaxe{Enchantments:[{id:efficiency,lvl:255}]} 1
```

## Protection 255 Armor

```mcfunction
/give @p diamond_chestplate{Enchantments:[{id:protection,lvl:255}]} 1
```

## Fortune 255 Pickaxe

```mcfunction
/give @p diamond_pickaxe{Enchantments:[{id:fortune,lvl:255}]} 1
```

---

# Full Netherite God Armor Example

## Helmet

```mcfunction
/give @p netherite_helmet{Enchantments:[{id:protection,lvl:255},{id:respiration,lvl:255},{id:aqua_affinity,lvl:1}]}
```

## Chestplate

```mcfunction
/give @p netherite_chestplate{Enchantments:[{id:protection,lvl:255},{id:unbreaking,lvl:255}]}
```

## Leggings

```mcfunction
/give @p netherite_leggings{Enchantments:[{id:protection,lvl:255},{id:swift_sneak,lvl:3}]}
```

## Boots

```mcfunction
/give @p netherite_boots{Enchantments:[{id:feather_falling,lvl:255},{id:depth_strider,lvl:255}]}
```

---

# Enchantment Tips

- Use `/enchant` for normal legal enchantments.
- Use `/give` with enchantment data for custom items.
- High-level enchantments can create extremely powerful items.
- Some enchantments cannot normally combine in survival.

---

More enchantment combinations and custom item commands will be added over time.
