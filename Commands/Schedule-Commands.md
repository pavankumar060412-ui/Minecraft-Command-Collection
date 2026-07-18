# Minecraft Schedule Commands

A collection of commands used to schedule delayed actions and automatic events in Minecraft.

# What Is The Schedule Command?

The `/schedule` command allows Minecraft functions to run after a specific amount of time.

It is mainly used for:
- Timers
- Automatic events
- Delayed actions
- Datapacks
- Server systems

---

# Schedule Function

## Run A Function After A Delay

```mcfunction
/schedule function <function> <time>
```

Example:

```mcfunction
/schedule function minecraft:test 10s
```

---

# Time Formats

## Seconds

```text
10s
```

## Minutes

```text
5m
```

## Hours

```text
1h
```

## Game Ticks

```text
200t
```

(20 ticks = 1 second)

---

# Schedule Examples

## Run Function After 10 Seconds

```mcfunction
/schedule function example:event 10s
```

## Run Function After 5 Minutes

```mcfunction
/schedule function example:event 5m
```

## Run Function After 1 Minute

```mcfunction
/schedule function example:event 1200t
```

---

# Clearing Scheduled Functions

## Remove A Scheduled Function

```mcfunction
/schedule clear <function>
```

Example:

```mcfunction
/schedule clear example:event
```

## Remove All Scheduled Functions

```mcfunction
/schedule clear *
```

---

# Timer Systems

## Delayed Message

Schedule:

```mcfunction
/schedule function example/message 10s
```

Function:

```mcfunction
/say Event started!
```

---

# Automatic Event Example

Start event:

```mcfunction
/schedule function example/end_event 5m
```

After the time:

```mcfunction
/say Event ended!
```

---

# Command Block Systems

Command blocks can trigger schedules:

```mcfunction
/schedule function example/reward 30s
```

After 30 seconds:

```mcfunction
/give @a diamond 1
```

---

# Uses Of Schedule Commands

Create:

- Countdown systems
- Boss events
- Server announcements
- Delayed traps
- Timed rewards
- Automatic resets
- Custom events

---

# Schedule Tips

- Schedule works best with functions.
- Use ticks for accurate timing.
- Combine with scoreboards for timers.
- Use datapacks for large systems.

---

More advanced scheduling systems will be added over time.
