# Minecraft Command Block Commands

A collection of commands and techniques used for creating automatic systems, machines, traps, and custom gameplay using command blocks.

# Getting Command Blocks

## Give Command Block

```mcfunction
/give @p command_block
```

## Give Repeating Command Block

```mcfunction
/give @p repeating_command_block
```

## Give Chain Command Block

```mcfunction
/give @p chain_command_block
```

---

# Command Block Types

## Impulse Command Block

- Runs a command once when activated.
- Used for buttons and levers.

## Repeat Command Block

- Runs a command continuously.
- Used for clocks and automatic systems.

## Chain Command Block

- Runs after another command block.
- Used for command sequences.

---

# Command Block Settings

## Needs Redstone

Requires a redstone signal.

## Always Active

Runs automatically without redstone.

## Conditional

Runs only if the previous command succeeds.

## Unconditional

Runs regardless of previous commands.

---

# Basic Command Block Examples

## Automatic Message

```mcfunction
/say Welcome to the server!
```

## Give Item When Activated

```mcfunction
/give @p diamond 1
```

## Teleport Player

```mcfunction
/tp @p 100 64 100
```

## Change Weather

```mcfunction
/weather clear
```

## Change Time

```mcfunction
/time set day
```

---

# Automatic Systems

## Automatic Night Vision

Command block:

```mcfunction
/effect give @a night_vision 10 1 true
```

Set to:

```
Repeat
Always Active
```

---

## Automatic Speed Boost

```mcfunction
/effect give @a speed 5 2 true
```

---

## Automatic Healing

```mcfunction
/effect give @a regeneration 5 1 true
```

---

# Teleport Systems

## Teleport Pad

Command:

```mcfunction
/tp @a[x=0,y=64,z=0,distance=..2] 100 70 100
```

Place in a repeating command block.

---

# Custom Messages

## Broadcast Message

```mcfunction
/say Server Event Starting!
```

## Colored Text

```mcfunction
/tellraw @a {"text":"Welcome!","color":"gold"}
```

---

# Command Block Traps

## TNT Trap

```mcfunction
/summon tnt ~ ~ ~ {Fuse:0}
```

## Lightning Trap

```mcfunction
/execute at @p run summon lightning_bolt
```

## Fire Trap

```mcfunction
/setblock ~ ~ ~ fire
```

---

# Mob Systems

## Automatic Mob Summoner

```mcfunction
/summon zombie ~ ~ ~
```

Set command block to repeat.

## Custom Boss Spawn

```mcfunction
/summon zombie ~ ~ ~ {CustomName:'{"text":"Boss"}'}
```

---

# Detection Commands

## Detect Player Near Block

```mcfunction
/execute if entity @p[distance=..5] run say Player detected
```

## Detect Player At Location

```mcfunction
/execute if entity @a[x=100,y=64,z=100,distance=..2] run say Found
```

---

# Execute Command Block Systems

## Run Command As Player

```mcfunction
/execute as @p run <command>
```

## Run Command At Location

```mcfunction
/execute at @p run <command>
```

## Combine Execute Commands

```mcfunction
/execute as @a at @s run <command>
```

---

# Minigame Commands

## Start Countdown

```mcfunction
/title @a title {"text":"3"}
```

## Give Players Items

```mcfunction
/give @a iron_sword
```

## Teleport Players

```mcfunction
/tp @a 0 100 0
```

## Clear Inventories

```mcfunction
/clear @a
```

---

# Custom Doors

## Open Door

```mcfunction
/setblock <x> <y> <z> air
```

## Close Door

```mcfunction
/setblock <x> <y> <z> iron_block
```

---

# Automatic Farms

## Automatic Crop Collection

Use:

```mcfunction
/execute
```

with:

```mcfunction
/kill @e[type=item]
```

for cleanup systems.

---

# Redstone + Command Block Tips

- Use repeating command blocks for automatic systems.
- Use chain command blocks for multiple actions.
- Use conditional blocks for advanced logic.
- Use `/execute` for powerful custom mechanics.
- Always test command systems in a backup world.

---

# Advanced Ideas

Create:
- Custom bosses
- Parkour maps
- Adventure maps
- Teleport networks
- Minigames
- Custom abilities
- RPG systems
- Automatic events

---

More command block machines and advanced systems will be added over time.
