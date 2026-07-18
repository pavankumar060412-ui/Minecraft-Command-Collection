# Minecraft Function Commands

A collection of commands used to create, run, and manage Minecraft functions.

# What Are Functions?

Functions are files containing multiple Minecraft commands that can be executed together.

They are useful for:
- Datapacks
- Automatic systems
- Command organization
- Server management
- Custom maps

---

# Function Command Basics

## Run A Function

```mcfunction
/function <function>
```

Example:

```mcfunction
/function minecraft:test
```

---

# Function Namespaces

Functions use namespaces:

```text
namespace:function_name
```

Example:

```mcfunction
/function example:start
```

---

# Creating Functions

Functions are stored inside datapacks:

```text
data/
 └── namespace/
     └── function/
         └── example.mcfunction
```

Example file:

```mcfunction
say Welcome!
give @p diamond 1
effect give @p speed 10 1
```

---

# Calling Functions

## Run A Function From A Command

```mcfunction
/function example/start
```

---

# Function With Command Blocks

Command block:

```mcfunction
/function example/event
```

The function can contain multiple commands.

---

# Automatic Functions

Functions can run automatically using:

- Load functions
- Tick functions
- Schedules

---

# Scheduled Functions

Run a function later:

```mcfunction
/schedule function example:event 10s
```

---

# Tick Functions

Tick functions run every game tick.

Useful for:

- Timers
- Machines
- Detection systems
- Custom abilities

---

# Function Examples

## Welcome Message

Function:

```mcfunction
say Welcome to the server!
```

Run:

```mcfunction
/function example:welcome
```

---

## Give Starter Items

Function:

```mcfunction
give @p stone_pickaxe
give @p bread 16
```

---

## Create A Boss Event

Function:

```mcfunction
summon zombie ~ ~ ~
tag @e[type=zombie,limit=1] add boss
effect give @e[tag=boss] strength 99999 5
```

---

# Function Tips

- Functions keep commands organized.
- Use namespaces to avoid conflicts.
- Combine functions with schedules and scoreboards.
- Datapacks rely heavily on functions.

---

More advanced function systems will be added over time.
