# Minecraft Server Setup Guide

A complete guide to creating, managing, and improving a Minecraft server.

# What Is A Minecraft Server?

A Minecraft server allows multiple players to play together in the same world.

Servers can be used for:

- Survival worlds
- SMPs
- Minigames
- Communities
- Private multiplayer

---

# Server Types

## Vanilla Server

The official Minecraft server software.

Features:

- Pure Minecraft experience
- No plugins
- No mods

Best for:

- Small survival servers

---

## Paper Server

A high-performance server software.

Features:

- Plugins
- Better performance
- More settings

Best for:

- SMP servers
- Communities

---

## Spigot Server

A plugin-based server platform.

Features:

- Bukkit plugins
- Custom gameplay

---

## Forge / NeoForge Server

Used for modded Minecraft.

Features:

- Mods
- Custom content
- New mechanics

---

# Creating A Server

## Requirements

Recommended:

```text
CPU:
Modern multi-core processor

RAM:
At least 4GB for small servers

Storage:
SSD recommended

Internet:
Stable connection
```

---

# Java Server Setup

Download the Minecraft server jar.

Create a folder:

```text
Minecraft Server
```

Place the server file inside.

Run:

```bash
java -jar server.jar
```

---

# Accepting EULA

Open:

```text
eula.txt
```

Change:

```text
eula=false
```

to:

```text
eula=true
```

---

# Starting The Server

Example:

```bash
java -Xmx4G -Xms2G -jar server.jar nogui
```

Explanation:

```text
-Xmx
Maximum RAM

-Xms
Starting RAM
```

---

# Server Properties

File:

```text
server.properties
```

Important settings:

---

## Server Name

```text
motd=My Minecraft Server
```

---

## Difficulty

```text
difficulty=normal
```

---

## Gamemode

```text
gamemode=survival
```

---

## Maximum Players

```text
max-players=20
```

---

## Online Mode

```text
online-mode=true
```

---

# Giving Yourself OP

In the server console:

```mcfunction
op PlayerName
```

---

# Useful Admin Commands

## Stop Server

```mcfunction
stop
```

---

## Teleport

```mcfunction
/tp player location
```

---

## Ban Player

```mcfunction
/ban player
```

---

## Whitelist

Enable:

```mcfunction
/whitelist on
```

Add player:

```mcfunction
/whitelist add PlayerName
```

---

# Plugins

Plugins add features to servers.

Popular plugins:

- EssentialsX
- LuckPerms
- WorldEdit
- WorldGuard
- CoreProtect

---

# Mods

Mods add new content.

Examples:

- Create
- Biomes O' Plenty
- JEI
- Mekanism

---

# Server Protection

Use:

- Backups
- Permissions
- Anti-grief plugins
- Whitelists

---

# Performance Optimization

Improve performance:

- Reduce render distance
- Use Paper
- Remove unnecessary entities
- Use SSD storage
- Optimize settings

---

# Backups

Always backup:

- World files
- Configuration files
- Plugins
- Mods

Example:

```text
world/
server.properties
plugins/
mods/
```

---

# Port Forwarding

For players outside your network:

Default port:

```text
25565
```

You may need to:

- Open router ports
- Configure firewall
- Share public IP

---

# Hosting Options

## Self Hosting

Run the server yourself.

Advantages:

- Full control
- Free

Disadvantages:

- Requires hardware
- Requires internet

---

## Server Hosting

Use a hosting company.

Advantages:

- Easy setup
- Better uptime

Disadvantages:

- Monthly cost

---

# Server Management Tips

- Keep backups.
- Update regularly.
- Protect player data.
- Use permissions.
- Monitor performance.

---

# Advanced Server Features

Create:

- Economy systems
- Custom worlds
- Minigames
- Events
- Ranks
- Shops

---

More advanced server guides will be added over time.
