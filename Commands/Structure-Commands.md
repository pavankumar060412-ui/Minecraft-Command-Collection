# Minecraft Structure Commands

A collection of commands used to save, load, and manage structures in Minecraft.

# What Are Structures?

Structures allow players to save builds and load them again later.

They are useful for:
- Copying builds
- Adventure maps
- Custom creations
- Server projects
- Reusable designs

---

# Structure Command Basics

## Save A Structure

```mcfunction
/structure save <name> <from> <to>
```

Example:

```mcfunction
/structure save house ~ ~ ~ ~10 ~10 ~10
```

---

# Load Structures

## Load A Structure

```mcfunction
/structure load <name>
```

Example:

```mcfunction
/structure load house
```

---

# Delete Structures

## Delete A Structure

```mcfunction
/structure delete <name>
```

Example:

```mcfunction
/structure delete house
```

---

# Structure Block Commands

## Give Structure Block

```mcfunction
/give @p structure_block
```

Structure blocks can:
- Save builds
- Load builds
- Export structures
- Rotate builds

---

# Structure Save Options

Structures can include:

- Blocks
- Entities
- Air blocks
- Custom builds

---

# Structure Load Options

## Load At Current Location

```mcfunction
/structure load house ~ ~ ~
```

## Load With Rotation

```mcfunction
/structure load house ~ ~ ~ 90_degrees
```

---

# Structure Examples

## Save A House

```mcfunction
/structure save house ~ ~ ~ ~20 ~15 ~20
```

## Load A House

```mcfunction
/structure load house
```

---

# Custom Map Uses

Create:

- Houses
- Dungeons
- Boss arenas
- Villages
- Redstone machines
- Adventure locations

---

# Structure Tips

- Use structure blocks for large builds.
- Save backups before loading structures.
- Structures can include mobs and entities.
- Combine structures with functions for automatic maps.

---

More advanced structure systems will be added over time.
