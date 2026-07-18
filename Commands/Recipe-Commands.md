# Minecraft Recipe Commands

A collection of commands used to manage crafting recipe unlocks in Minecraft.

# What Is The Recipe Command?

The `/recipe` command allows players and administrators to control which crafting recipes are unlocked or removed.

It is useful for:
- Custom survival challenges
- Adventure maps
- Progression systems
- Restricted crafting worlds

---

# Unlock Recipes

## Unlock A Specific Recipe

```mcfunction
/recipe give <player> <recipe>
```

Example:

```mcfunction
/recipe give @p minecraft:diamond_sword
```

---

## Unlock All Recipes

```mcfunction
/recipe give <player> *
```

Example:

```mcfunction
/recipe give @p *
```

---

# Remove Recipes

## Remove A Specific Recipe

```mcfunction
/recipe take <player> <recipe>
```

Example:

```mcfunction
/recipe take @p minecraft:diamond_sword
```

---

## Remove All Recipes

```mcfunction
/recipe take <player> *
```

Example:

```mcfunction
/recipe take @p *
```

---

# Recipe Examples

## Unlock Crafting Table

```mcfunction
/recipe give @p minecraft:crafting_table
```

## Unlock Furnace

```mcfunction
/recipe give @p minecraft:furnace
```

## Unlock Diamond Sword

```mcfunction
/recipe give @p minecraft:diamond_sword
```

## Unlock Netherite Sword

```mcfunction
/recipe give @p minecraft:netherite_sword
```

## Unlock Golden Apple

```mcfunction
/recipe give @p minecraft:golden_apple
```

---

# Custom Progression Systems

## Remove All Recipes At Start

```mcfunction
/recipe take @a *
```

Then unlock recipes as players progress:

```mcfunction
/recipe give @a minecraft:iron_pickaxe
```

---

# Adventure Map Example

Beginning of map:

```mcfunction
/recipe take @p *
```

After completing a quest:

```mcfunction
/recipe give @p minecraft:diamond_pickaxe
```

---

# Command Block Recipe Systems

## Recipe Unlock Button

```mcfunction
/recipe give @p minecraft:bow
```

---

# Recipe Ideas

Use recipe commands for:

- RPG progression
- Custom survival modes
- Quest rewards
- Tutorial maps
- Challenge worlds
- Server events

---

# Recipe Tips

- Recipe names use Minecraft IDs.
- Use `*` carefully because it affects every recipe.
- Combine recipes with advancements for progression.
- Datapacks allow fully custom recipes.

---

More recipe systems and custom crafting examples will be added over time.
