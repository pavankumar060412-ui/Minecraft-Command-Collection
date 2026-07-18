# Minecraft Redstone Guide

A complete guide to understanding and creating redstone systems in Minecraft.

# What Is Redstone?

Redstone is Minecraft's power system that allows players to create machines, circuits, and automatic farms.

Redstone can be used for:

- Doors
- Farms
- Traps
- Machines
- Clocks
- Sorting systems
- Automated builds

---

# Basic Redstone Components

## Redstone Dust

Redstone dust carries power between components.

Example uses:

- Connecting circuits
- Powering blocks
- Creating signals

---

## Redstone Torch

A redstone torch provides power and can also invert signals.

Uses:

- Logic gates
- Automatic doors
- Circuits

---

## Lever

A manual switch that gives a constant redstone signal.

Example:

```mcfunction
/setblock ~ ~ ~ lever
```

---

## Button

Provides a short redstone pulse when pressed.

Used for:

- Doors
- Commands
- Machines

---

## Pressure Plate

Activates when an entity stands on it.

Used for:

- Hidden doors
- Traps
- Automatic systems

---

# Redstone Power

Redstone signals travel up to:

```text
15 blocks
```

After that, the signal needs a repeater.

---

# Redstone Repeater

Repeaters:

- Extend signal distance
- Add delays
- Control timing

Example:

```text
Redstone → Repeater → Redstone
```

---

# Redstone Comparator

Comparators are used for:

- Measuring containers
- Comparing signals
- Advanced circuits

Common uses:

- Sorting systems
- Item detectors
- Storage systems

---

# Pistons

## Normal Piston

Pushes blocks.

Uses:

- Doors
- Farms
- Machines

---

## Sticky Piston

Pulls blocks back after pushing.

Uses:

- Hidden doors
- Moving machines

---

# Redstone Doors

Basic piston door:

Components:

- Pistons
- Redstone dust
- Pressure plate/button

System:

```text
Input → Redstone → Pistons → Door Opens
```

---

# Redstone Clocks

A redstone clock creates repeated signals.

Used for:

- Automatic farms
- Machines
- Timers

---

# Hopper Systems

Hoppers move and store items automatically.

Uses:

- Item collection
- Storage systems
- Sorting machines

Example:

```text
Chest
 ↓
Hopper
 ↓
Chest
```

---

# Automatic Farms

Redstone can automate:

- Sugar cane farms
- Bamboo farms
- Pumpkin farms
- Melon farms
- Crop farms

Common components:

- Observers
- Pistons
- Hoppers
- Water

---

# Observers

Observers detect block changes.

Uses:

- Automatic farms
- Flying machines
- Detection systems

Example:

```text
Block Change
      ↓
 Observer
      ↓
 Redstone Signal
```

---

# Command Block Redstone Systems

Redstone can activate commands.

Example:

```mcfunction
/give @p diamond
```

Activated by:

- Buttons
- Levers
- Pressure plates

---

# Advanced Redstone Builds

Examples:

- Hidden bases
- Elevators
- Traps
- Automatic doors
- Sorting systems
- Machines
- Minigames

---

# Redstone Tips

- Keep circuits organized.
- Use repeaters for long distances.
- Test machines in creative mode first.
- Use observers for automatic detection.
- Learn basic logic gates for advanced builds.

---

More advanced redstone systems will be added over time.
