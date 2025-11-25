# PaperMC Server Admin & Moderator Command Cheat Sheet
## Complete Guide for Server Administrators and Moderators

---

## 👮 MODERATOR COMMANDS (Player Management & Moderation)

### Essential Moderation (EssentialsX)

| Command | Description | Permission |
|---------|-------------|-----------|
| `/kick [player] [reason]` | Kicks a player from the server (they can rejoin) | essentials.kick |
| `/ban [player] [reason]` | Permanently bans a player | essentials.ban |
| `/tempban [player] [time] [reason]` | Temporarily bans a player (e.g., `/tempban player 7d Griefing`) | essentials.tempban |
| `/unban [player]` | Unbans a player | essentials.unban |
| `/mute [player]` | Permanently silences a player's chat | essentials.mute |
| `/tempmute [player] [time] [reason]` | Temporarily mutes a player | essentials.tempmute |
| `/unmute [player]` | Unmutes a player | essentials.unmute |
| `/warn [player] [reason]` | Warns a player (visible to them) | essentials.warn |

### Player Investigation & Monitoring

| Command | Description | Permission |
|---------|-------------|-----------|
| `/invsee [player]` | View (and edit) a player's inventory remotely | essentials.invsee |
| `/enderchest [player]` | Opens a player's Ender Chest to inspect | essentials.enderchest |
| `/whois [player]` | Shows detailed info about a player (IPs, last online, etc.) | essentials.whois |
| `/seen [player]` | Shows when a player was last online | essentials.seen |
| `/socialspy` | Toggle PM spy mode (see all private messages) | essentials.socialspy |
| `/chat spy` | Toggles chat spy for monitoring conversations | essentials.chat.spy |

### Player Teleportation & Control

| Command | Description | Permission |
|---------|-------------|-----------|
| `/tp [player1] [player2]` | Teleports player1 to player2's location | essentials.tp |
| `/tpall` | Teleports all online players to you | essentials.tpall |
| `/teleport [player] [x] [y] [z]` | Teleports a player to specific coordinates | essentials.teleport |
| `/bring [player]` | Brings a player to your location | essentials.tp |
| `/freeze [player]` | Freezes a player in place (prevents movement) | essentials.freeze |
| `/vanish` | Hides you from all players (appear offline) | essentials.vanish |
| `/paytoggle` | Blocks receiving money payments | essentials.paytoggle |

### Player Utilities

| Command | Description | Permission |
|---------|-------------|-----------|
| `/nickother [player] [name]` | Sets another player's nickname | essentials.nickother |
| `/clearinventory [player]` | Clears a player's inventory | essentials.clearinventory |
| `/heal [player]` | Heals a player to full health | essentials.heal |
| `/feed [player]` | Fills a player's hunger bar | essentials.feed |
| `/suicide` | Removes a player from the server gracefully | essentials.suicide |

---

## 🛠️ ADMIN COMMANDS (Server Management)

### Operator Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/op [player]` | Makes a player a server operator (grants all permissions) | bukkit.command.op |
| `/deop [player]` | Removes operator status from a player | bukkit.command.deop |
| `/ops` | Lists all current operators | bukkit.command.ops |

### Server Control & Configuration

| Command | Description | Permission |
|---------|-------------|-----------|
| `/stop` | Stops the server gracefully | bukkit.command.stop |
| `/restart` | Restarts the server | bukkit.command.restart |
| `/save-all` | Forces the server to save all data | bukkit.command.save-all |
| `/save-off` | Disables auto-saving (not recommended) | bukkit.command.save-off |
| `/save-on` | Re-enables auto-saving | bukkit.command.save-on |
| `/reload` | Reloads all server configs and plugins | bukkit.command.reload |
| `/reload confirm` | Confirms reload (required after first reload command) | bukkit.command.reload |

### Difficulty & Gamemode Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/difficulty [peaceful\|easy\|normal\|hard]` | Changes server difficulty | bukkit.command.difficulty |
| `/gamemode [mode] [player]` | Changes gamemode (survival, creative, adventure, spectator) | bukkit.command.gamemode |
| `/defaultgamemode [mode]` | Sets the default gamemode for new players | bukkit.command.defaultgamemode |

### World & Time Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/time set [time]` | Sets world time (0-24000, or "day"/"night") | bukkit.command.time |
| `/time add [amount]` | Adds time to current world time | bukkit.command.time |
| `/weather [clear\|rain\|thunder]` | Changes weather | bukkit.command.weather |
| `/seed` | Shows the current world seed | bukkit.command.seed |

### Whitelist Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/whitelist on` | Enables the whitelist (only whitelisted players can join) | bukkit.command.whitelist |
| `/whitelist off` | Disables the whitelist | bukkit.command.whitelist |
| `/whitelist add [player]` | Adds a player to the whitelist | bukkit.command.whitelist |
| `/whitelist remove [player]` | Removes a player from the whitelist | bukkit.command.whitelist |
| `/whitelist list` | Lists all whitelisted players | bukkit.command.whitelist |
| `/whitelist reload` | Reloads the whitelist from file | bukkit.command.whitelist |

### Ban Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/banlist` | Shows all banned players | bukkit.command.banlist |
| `/banlist ips` | Shows all banned IP addresses | bukkit.command.banlist |
| `/pardon [player]` | Unbans a player (alias for /unban) | bukkit.command.unban |
| `/pardon-ip [ip]` | Unbans an IP address | bukkit.command.unbanip |
| `/ban-ip [player\|ip]` | Bans a player's IP address | bukkit.command.ban-ip |

### Item & Inventory Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/give [player] [item] [amount] [data]` | Gives a player an item | bukkit.command.give |
| `/clear [player] [item] [amount]` | Clears items from a player's inventory | bukkit.command.clear |
| `/enchant [player] [enchantment] [level]` | Enchants an item in a player's hand | bukkit.command.enchant |
| `/item` | Opens item editor interface | bukkit.command.item |

### Teleportation Commands

| Command | Description | Permission |
|---------|-------------|-----------|
| `/teleport [player] [x] [y] [z]` | Teleports to coordinates | bukkit.command.teleport |
| `/teleport [player] [rotation]` | Teleports with rotation control | bukkit.command.teleport |
| `/teleport [player1] [player2]` | Teleports player1 to player2 | bukkit.command.teleport |

### Coordinate & Locating

| Command | Description | Permission |
|---------|-------------|-----------|
| `/locate [biome\|structure]` | Locates nearest biome or structure | bukkit.command.locate |
| `/locatebiome [biome]` | Finds nearest biome | bukkit.command.locatebiome |
| `/spreadplayers [x] [z] [distance] [max-range] [player...]` | Spreads players across a large area | bukkit.command.spreadplayers |

### Entity Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/summon [entity] [x] [y] [z] [nbt]` | Spawns an entity at specified location | bukkit.command.summon |
| `/kill [player\|entity]` | Kills a player or entity | bukkit.command.kill |
| `/setblock [x] [y] [z] [block]` | Changes a single block at location | bukkit.command.setblock |

### Data & NBT Commands

| Command | Description | Permission |
|---------|-------------|-----------|
| `/data modify` | Modifies NBT data of entities/blocks | bukkit.command.data |
| `/scoreboard` | Manages scoreboards and objectives | bukkit.command.scoreboard |

---

## 🔐 LUCKPERMS ADMIN COMMANDS (Permission Management)

### User Management

| Command | Description |
|---------|-------------|
| `/lp user [name] info` | Shows all permissions and groups for a user |
| `/lp user [name] parent set [group]` | Assigns a user to a group |
| `/lp user [name] parent add [group]` | Adds a user to a group (keeps other groups) |
| `/lp user [name] parent remove [group]` | Removes a user from a group |
| `/lp user [name] permission set [permission] true` | Grants a specific permission to a user |
| `/lp user [name] permission set [permission] false` | Denies a specific permission from a user |
| `/lp user [name] permission unset [permission]` | Removes a permission from a user |
| `/lp user [name] promote [track]` | Promotes a user up one rank in a track |
| `/lp user [name] demote [track]` | Demotes a user down one rank in a track |

### Group Management

| Command | Description |
|---------|-------------|
| `/lp group [name] create` | Creates a new group |
| `/lp group [name] delete` | Deletes a group |
| `/lp group [name] info` | Shows group information |
| `/lp group [name] permission set [permission] true` | Grants permission to group |
| `/lp group [name] permission unset [permission]` | Removes permission from group |
| `/lp group [name] parent add [parent]` | Sets group inheritance |
| `/lp group [name] parent remove [parent]` | Removes group inheritance |

### Track Management

| Command | Description |
|---------|-------------|
| `/lp track [name] create` | Creates a new promotion track |
| `/lp track [name] append [group]` | Adds a group to the end of a track |
| `/lp track [name] insert [position] [group]` | Inserts a group into a track at specific position |
| `/lp track [name] remove [group]` | Removes a group from a track |
| `/lp track [name] info` | Shows track information |

### Web Editor

| Command | Description |
|---------|-------------|
| `/lp editor` | Opens the LuckPerms web editor (visual GUI for permissions) |

---

## 📊 SPARK (Performance Diagnostics)

### Server Diagnostics

| Command | Description | Permission |
|---------|-------------|-----------|
| `/spark tps` | Shows server TPS (ticks per second) and CPU usage | spark.tps |
| `/spark health` | Generates comprehensive server health report | spark.healthreport |
| `/spark health --upload` | Uploads health report and returns shareable link | spark.healthreport |
| `/spark info` | Shows basic server information | spark.info |
| `/spark ping [player]` | Shows a player's ping/latency | spark.ping |

### Profiling (Finding Lag Sources)

| Command | Description | Permission |
|---------|-------------|-----------|
| `/spark profiler start` | Starts CPU profiler (30 seconds default) | spark.profiler |
| `/spark profiler start --timeout 60` | Starts profiler for 60 seconds | spark.profiler |
| `/spark profiler stop` | Stops profiler and uploads results | spark.profiler |
| `/spark profiler cancel` | Stops profiler without uploading | spark.profiler |
| `/spark profiler info` | Shows current profiler status | spark.profiler |

### Memory Analysis

| Command | Description | Permission |
|---------|-------------|-----------|
| `/spark gc` | Shows garbage collection history | spark.gc |
| `/spark gcmonitor` | Toggles GC monitoring | spark.gcmonitor |
| `/spark heapsummary` | Creates memory (heap) dump analysis | spark.heapsummary |

### Tick Monitoring

| Command | Description | Permission |
|---------|-------------|-----------|
| `/spark tickmonitor` | Toggles tick duration monitoring | spark.tickmonitor |
| `/spark tickmonitor --threshold 50` | Monitor ticks above 50% threshold | spark.tickmonitor |

---

## 🏘️ TOWNY ADMIN COMMANDS (Town & Nation Management)

### Town Administration

| Command | Description | Permission |
|---------|-------------|-----------|
| `/t purge [town]` | Deletes a town completely | towny.admin.delete.town |
| `/t delete [town]` | Deletes a town | towny.admin.delete.town |
| `/t resetpeace` | Removes all towns from peace mode | towny.admin.town.resetpeace |
| `/t unclaim [town] [all]` | Unclaims all land for a town | towny.admin.unclaim.town |
| `/t toggle [townblock] [toggle]` | Enables/disables explosions, PvP, fire in a town | towny.admin.toggle |

### Nation Administration

| Command | Description | Permission |
|---------|-------------|-----------|
| `/n purge [nation]` | Deletes a nation completely | towny.admin.delete.nation |
| `/n delete [nation]` | Deletes a nation | towny.admin.delete.nation |
| `/n resetpeace` | Removes all nations from peace mode | towny.admin.nation.resetpeace |

### Player & Plot Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/plot set title [name]` | Sets a plot's title | towny.admin.plot |
| `/plot set perm [type]` | Modifies plot permissions | towny.admin.plot.perm |
| `/plot claim [town]` | Force-claims a plot for a town | towny.admin.claim.plot |
| `/plot unclaim [town]` | Force-unclaims a plot from a town | towny.admin.unclaim.plot |

---

## 💰 ESSENTIALS ECONOMY ADMIN COMMANDS

### Player Money Management

| Command | Description | Permission |
|---------|-------------|-----------|
| `/eco give [player] [amount]` | Gives money to a player | essentials.eco.give |
| `/eco take [player] [amount]` | Takes money from a player | essentials.eco.take |
| `/eco set [player] [amount]` | Sets a player's balance to exact amount | essentials.eco.set |
| `/eco reset [player]` | Resets a player's balance to starting balance | essentials.eco.reset |

### Economy Info

| Command | Description | Permission |
|---------|-------------|-----------|
| `/money top [page]` | Shows richest players | essentials.money.top |
| `/money other [player]` | Checks another player's balance | essentials.money.other |

---

## 📝 USEFUL ADMIN CONSOLE-ONLY COMMANDS

These commands should be typed in your **server console**, not in-game:

### Plugin Management

```
/plugins                 # Shows all loaded plugins
/reload                  # Reloads all plugins and configs
/pl                      # Short version of /plugins
/plugin reload [name]    # Reloads specific plugin
```

### Server Management (Console)

```
say [message]            # Broadcasts a message to all players
list                     # Lists all online players
op [player]              # Makes someone operator
deop [player]            # Removes operator status
stop                     # Stops the server
restart                  # Restarts the server
```

### Debugging (Console)

```
debug start              # Starts server debug profiler
debug stop               # Stops and shows debug results
jps                      # Shows Java process status (Linux)
```

---

## 🎯 MODERATOR WORKFLOW (Common Scenarios)

### Dealing with a Spammer

1. `/mute [player]` - Silences them immediately
2. `/invsee [player]` - Check if they're using bots/hacks
3. `/warn [player] Excessive spam` - Add warning
4. If persistent: `/kick [player] Continued spam`
5. If very bad: `/tempban [player] 1h Spam`

### Investigating a Griefer

1. `/seen [griefer]` - When were they last online?
2. `/whois [griefer]` - Get their info
3. `/invsee [griefer]` - Check inventory for stolen items
4. `/vanish` - Hide yourself and observe
5. `/ban [griefer] Griefing` or `/tempban [griefer] 7d Griefing`

### Managing Disruptive Players

1. `/socialspy` - Listen to their PMs (if selling exploits)
2. `/kick [player] Reason` - First offense
3. `/tempban [player] 1h Reason` - Second offense
4. `/ban [player] Repeated violations` - Permanent ban if needed

---

## ⚙️ ADVANCED ADMIN TASKS

### Creating a VIP Kit

1. Set up your VIP inventory exactly how you want it
2. `/createkit vip` - Creates the kit
3. `/lp group vip permission set essentials.kit.vip true` - Allow VIPs to use it

### Setting Command Costs

Edit `/plugins/Essentials/config.yml`:

```yaml
command-costs:
  home: 100
  warp: 50
  fly: 250
  spawn: 0
```

### Banning an IP Address

```
/ban-ip 123.45.67.89 Banned for hacking
```

### Teleporting All Players to Event Location

```
/tpall
```
This brings everyone to you.

### Clearing All Dropped Items

```
/kill @e[type=item]
```

### Broadcasting Important Messages

```
/say ===== SERVER MAINTENANCE IN 5 MINUTES =====
/say All players will be kicked for restart
/say Please save your progress!
```

---

## 📞 TROUBLESHOOTING

### Players Can't Use Commands They Should Have Access To

1. Check they're in the right group: `/lp user [name] info`
2. Verify permission is set: Look for the permission in the list
3. Reload LuckPerms: `/lp user [name] parent set [group]` again
4. Restart server if still broken

### Need to Quickly Grant Admin Access

```
/op [playername]
```

This gives them full access immediately (use with caution).

### Player Keeps Rejoining After Ban

```
/ban-ip [their-ip-address] Ban reason
```

This bans their IP, preventing all their accounts from joining.

### Server Performance Issues

```
/spark tps              # Check TPS first
/spark health --upload  # Get full report
```

Then share the link with technical support.

---

## 📋 PERMISSION QUICK REFERENCE

**Moderators need:**
- essentials.kick
- essentials.ban
- essentials.tempban
- essentials.mute
- essentials.invsee
- essentials.tp
- spark.* (for diagnostics)

**Admins need:**
- bukkit.command.* (all vanilla commands)
- essentials.* (all EssentialsX commands)
- luckperms.* (all permission management)
- towny.admin.* (all town admin)
- spark.* (all diagnostics)

---

Good luck managing your server! Remember: **With great power comes great responsibility.** Use these tools wisely and fairly. 🎮⚔️