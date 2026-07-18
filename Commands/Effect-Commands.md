# Minecraft Effect Commands

A collection of commands used to apply, remove, and manage status effects in Minecraft.

# Basic Effect Commands

## Give An Effect

```mcfunction
/effect give <player> <effect> <duration> <amplifier>
```

Example:

```mcfunction
/effect give @p speed 60 5
```

## Remove All Effects

```mcfunction
/effect clear <player>
```

Example:

```mcfunction
/effect clear @p
```

## Remove A Specific Effect

```mcfunction
/effect clear <player> <effect>
```

Example:

```mcfunction
/effect clear @p speed
```

---

# Movement Effects

## Speed

```mcfunction
/effect give @p speed 99999 5
```

## Slowness

```mcfunction
/effect give @p slowness 99999 5
```

## Jump Boost

```mcfunction
/effect give @p jump_boost 99999 5
```

## Slow Falling

```mcfunction
/effect give @p slow_falling 99999 1
```

---

# Combat Effects

## Strength

```mcfunction
/effect give @p strength 99999 5
```

## Weakness

```mcfunction
/effect give @p weakness 99999 5
```

## Resistance

```mcfunction
/effect give @p resistance 99999 5
```

## Absorption

```mcfunction
/effect give @p absorption 99999 5
```

## Regeneration

```mcfunction
/effect give @p regeneration 99999 5
```

---

# Vision Effects

## Night Vision

```mcfunction
/effect give @p night_vision 99999 1
```

## Blindness

```mcfunction
/effect give @p blindness 99999 1
```

## Darkness

```mcfunction
/effect give @p darkness 99999 1
```

---

# Environment Effects

## Fire Resistance

```mcfunction
/effect give @p fire_resistance 99999 1
```

## Water Breathing

```mcfunction
/effect give @p water_breathing 99999 1
```

## Invisibility

```mcfunction
/effect give @p invisibility 99999 1
```

## Conduit Power

```mcfunction
/effect give @p conduit_power 99999 1
```

---

# Mining Effects

## Haste

```mcfunction
/effect give @p haste 99999 5
```

## Mining Fatigue

```mcfunction
/effect give @p mining_fatigue 99999 5
```

---

# Special Effects

## Glowing

```mcfunction
/effect give @p glowing 99999 1
```

## Levitation

```mcfunction
/effect give @p levitation 10 5
```

## Luck

```mcfunction
/effect give @p luck 99999 5
```

## Bad Luck

```mcfunction
/effect give @p unluck 99999 5
```

## Hero Of The Village

```mcfunction
/effect give @p hero_of_the_village 99999 1
```

## Bad Omen

```mcfunction
/effect give @p bad_omen 99999 1
```

---

# Effects For All Players

## Give Everyone Night Vision

```mcfunction
/effect give @a night_vision 99999 1
```

## Give Everyone Speed

```mcfunction
/effect give @a speed 99999 3
```

## Remove All Player Effects

```mcfunction
/effect clear @a
```

---

# Effects For Mobs

## Give All Zombies Strength

```mcfunction
/effect give @e[type=zombie] strength 99999 5
```

## Give All Mobs Speed

```mcfunction
/effect give @e[type=!player] speed 99999 3
```

## Remove Effects From All Entities

```mcfunction
/effect clear @e
```

---

# Advanced Effect Commands

## Infinite Effect

Use a very high duration:

```mcfunction
/effect give @p speed 999999 5
```

## Maximum Effect Level

```mcfunction
/effect give @p strength 999999 255
```

## Effect A Specific Entity

```mcfunction
/effect give @e[type=minecraft:warden] resistance 100 5
```

---

# Useful Effect Combinations

## Super Miner

```mcfunction
/effect give @p haste 99999 5
/effect give @p night_vision 99999 1
```

## Fast Runner

```mcfunction
/effect give @p speed 99999 5
/effect give @p jump_boost 99999 3
```

## Fireproof Player

```mcfunction
/effect give @p fire_resistance 99999 1
```

## Underwater Explorer

```mcfunction
/effect give @p water_breathing 99999 1
/effect give @p night_vision 99999 1
```

---

# Effect Tips

- Amplifier levels start at 0 internally, so level 5 uses amplifier 4 in some situations.
- Use long durations for permanent abilities.
- Combine effects with command blocks for custom game modes.
- Always test powerful effects before using them on servers.

---

More effect combinations and advanced potion systems will be added over time.
