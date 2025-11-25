# PaperMC Server Command Cheat Sheet
## Complete Player Command Guide for Your Server

---

## 🎮 ESSENTIAL COMMANDS (EssentialsX)

### Teleportation & Navigation
| Command | Description |
|---------|-------------|
| `/spawn` | Teleports you to the server spawn point |
| `/home` | Teleports you to your set home |
| `/sethome [name]` | Sets your current location as home (can have multiple) |
| `/delhome [name]` | Deletes a home |
| `/homes` | Lists all your saved homes |
| `/warp [name]` | Teleports to a public warp point |
| `/warp list` | Lists all available warps |
| `/back` | Returns to your previous location |
| `/tpa [player]` | Requests to teleport to another player |
| `/tpaccept` | Accepts a teleport request |
| `/tpdeny` | Denies a teleport request |

### Communication
| Command | Description |
|---------|-------------|
| `/msg [player] [message]` | Sends a private message to a player |
| `/reply [message]` | Quick reply to the last person who messaged you |
| `/mail send [player] [message]` | Sends mail to an offline player |
| `/mail read` | Reads your mail |
| `/mail clear` | Clears all your mail |

### Player Information
| Command | Description |
|---------|-------------|
| `/list` | Shows all players currently online |
| `/whois [player]` | Shows info about a player |
| `/seen [player]` | Shows when a player was last online |
| `/help` | Shows a list of available commands |
| `/rules` | Shows the server rules |
| `/motd` | Shows the message of the day |
| `/info` | Shows server information |

### Gameplay & Utilities
| Command | Description |
|---------|-------------|
| `/nick [name]` | Changes your displayed nickname (VIP+ only) |
| `/fly` | Enables/disables flying mode (VIP+ only) |
| `/exp` | Shows your current XP amount |
| `/hat` | Places the block in your hand on your head (VIP+ only) |
| `/repair` | Repairs the item in your hand (VIP+ only) |
| `/workbench` | Opens a crafting table anywhere (VIP+ only) |
| `/afk` | Sets yourself as AFK (away from keyboard) |

---

## 💰 ECONOMY COMMANDS (TheNewEconomy + VaultUnlocked)

### Money Management
| Command | Description |
|---------|-------------|
| `/money balance` | Shows your current balance |
| `/bal` | Shortcut for balance |
| `/money pay [player] [amount]` | Sends money to another player |
| `/money top [page]` | Shows the richest players on the server |
| `/money history [page]` | Shows your transaction history |
| `/money other [player]` | Checks another player's balance (admins only) |

### Economy Features
| Command | Description |
|---------|-------------|
| `/money note [amount]` | Converts virtual money into a physical note item for trading |
| `/money request [player] [amount]` | Requests money from a player |
| `/money convert [amount] [currency]` | Converts money between currencies |
| `/money away [page]` | Shows transactions you missed while offline |

---

## 🏘️ TOWN & NATION MANAGEMENT (Towny)

### Town Basics
| Command | Description |
|---------|-------------|
| `/town` | Shows your town's status and info |
| `/town new [name]` | Creates a new town |
| `/town info [town]` | Shows info about a specific town |
| `/town list` | Lists all towns on the server |
| `/town here` | Shows town info about your current location |
| `/town leave` | Leaves your current town |
| `/town online` | Shows online members in your town |

### Town Management (Mayor/Co-Mayor)
| Command | Description |
|---------|-------------|
| `/town add [player]` | Adds a player to your town |
| `/town kick [player]` | Removes a player from your town |
| `/town set spawn` | Sets town spawn at your current location |
| `/town set name [name]` | Renames your town |
| `/town set tag [tag]` | Sets a short town tag (4 characters max) |
| `/town claim` | Claims a chunk for your town |
| `/town unclaim` | Unclaims a chunk from your town |
| `/town rank add [player] [rank]` | Adds a rank to a town member |
| `/town rank remove [player] [rank]` | Removes a rank from a town member |

**Available Town Ranks:** Mayor, Co-Mayor, Helper, Sheriff

### Town Finances (Mayor)
| Command | Description |
|---------|-------------|
| `/town bank` | Shows your town's bank balance |
| `/town bank deposit [amount]` | Deposits money into town bank |
| `/town bank withdraw [amount]` | Withdraws money from town bank |
| `/town set taxes [amount]` | Sets daily tax for residents |

### Town Chat
| Command | Description |
|---------|-------------|
| `/tc [message]` | Sends a message to all town members online |
| `/tcmute` | Mutes town chat (admin only) |

### Resident Commands
| Command | Description |
|---------|-------------|
| `/resident` | Shows your resident information |
| `/resident [player]` | Shows another player's resident info |
| `/res list` | Lists all residents |
| `/res friend add [player]` | Adds a friend to your friend list |
| `/res friend remove [player]` | Removes a friend |
| `/res toggle map` | Toggles auto map view in chat |
| `/res toggle townclaim` | Toggles auto town claiming mode |

### Nations (Advanced)
| Command | Description |
|---------|-------------|
| `/nation` | Shows your nation's status |
| `/nation new [name]` | Creates a new nation |
| `/nation info [nation]` | Shows info about a nation |
| `/nation list` | Lists all nations |
| `/nation add [town]` | Adds your town to a nation (King+ only) |
| `/nation kick [town]` | Removes a town from nation (King+ only) |
| `/nation leave` | Your town leaves the nation |
| `/nation set spawn` | Sets nation spawn (King+ only) |
| `/nation spawn [nation]` | Teleports to nation spawn |
| `/nation bank` | Shows nation bank (King+ only) |
| `/nation bank deposit [amount]` | Deposits to nation bank (King+ only) |
| `/nc [message]` | Sends message to all nation members online |

**Available Nation Ranks:** King, Assistant, Helper

---

## ⚔️ SKILLS & PROGRESSION (AuraSkills)

### Skills Menu & Information
| Command | Description |
|---------|-------------|
| `/skills` | Opens the skills menu showing all your skills |
| `/stats` | Opens stats menu showing your stat levels |
| `/[skill]` | Opens a specific skill menu (e.g., `/mining`, `/farming`) |
| `/sk top [page]` | Shows leaderboard of top players overall |
| `/sk top [skill]` | Shows leaderboard for a specific skill |
| `/sk rank` | Shows your personal skill rankings |
| `/skilltop [page]` | Shortcut for skill top leaderboard |
| `/skillrank` | Shortcut for skill rank |

### Mana & Resources
| Command | Description |
|---------|-------------|
| `/mana` | Shows your current mana amount |

### Settings
| Command | Description |
|---------|-------------|
| `/abtoggle` | Toggles the action bar display on/off |
| `/sk toggle` | Same as abtoggle |
| `/sk lang [language]` | Changes your language for messages |
| `/sk claimitems` | Opens menu to claim rewards that didn't fit in inventory |

### Skill Sources
| Command | Description |
|---------|-------------|
| `/sk sources [skill]` | Shows all ways to gain XP for a skill |

---

## 🔍 PERFORMANCE & DIAGNOSTICS (Spark)

### Profiling Commands
| Command | Description |
|---------|-------------|
| `/spark info` | Shows basic server info |
| `/spark stats` | Shows memory and tick stats |
| `/spark profiler start` | Starts a CPU profiler session |
| `/spark profiler stop` | Stops and shows profiler results |
| `/spark tickmonitoring start` | Starts monitoring tick durations |
| `/spark tickmonitoring stop` | Stops tick monitoring |

---

## 🎯 PLACEHOLDERS & CHAT (PlaceholderAPI)

### Chat Formatting
You can use special characters in your messages with the right permissions:

| Code | Effect |
|------|--------|
| `&c` | Red text |
| `&a` | Green text |
| `&b` | Cyan text |
| `&6` | Gold text |
| `&f` | White text |
| `&l` | **Bold** |
| `&o` | *Italic* |
| `&n` | Underline |

**Example:** `/nick &c&lCoolName` creates a bold red nickname

---

## 📊 QUICK REFERENCE BY RANK

### Default Players
- Basic chat, help, rules, motd
- `/spawn`, `/tpa`, `/msg`
- `/money balance`
- `/town list`, `/town info`
- `/skills`, `/sk top`

### Members
- Everything from Default +
- `/home`, `/sethome`, `/delhome`
- `/warp`, `/back`
- `/town new`, town management basics
- `/money pay`

### VIPs
- Everything from Member +
- `/fly`, `/hat`, `/repair`, `/workbench`
- Multiple homes (`/sethome [name]`)
- Custom nickname (`/nick`)
- `/money convert`

### Moderators
- Everything from VIP +
- Moderation commands (handled separately)
- Access to `/spark` diagnostics
- `/town` admin commands
- Server management tools

### Admins
- Full access to ALL commands
- Ability to modify any setting
- Server control and configuration

---

## ⚠️ TIPS & TRICKS

### Money Tips
- Use `/money history` to track transactions
- Convert money to notes with `/money note` for safe storage
- Check `/money top` to see if you're getting rich!

### Town Tips
- Use `/town claim` to protect your land
- Create a town spawn with `/town set spawn`
- Invite friends with `/town add`
- Join a nation for extra perks!

### Skills Tips
- Visit `/[skill]` to see how to level up that skill
- Use `/sk sources [skill]` to find the best XP farming method
- Check `/sk top` to compete with other players
- Toggle your action bar with `/abtoggle` if you find it annoying

### General Tips
- You can set multiple homes with different names: `/sethome base`, `/sethome farm`
- Use `/tpa` to avoid forced teleports—always ask first!
- Check `/seen [player]` to know when your friends were last online
- Private message someone with `/msg [player] [message]`

---

## ❓ COMMON QUESTIONS

**Q: I don't have enough homes!**
A: Buy a VIP rank to get multiple homes, or ask an admin to increase your home limit.

**Q: How do I make money?**
A: Gain skill XP by doing tasks (mining, farming, etc.), then sell items or complete tasks.

**Q: How do I create a town?**
A: Use `/town new [name]` then `/town set spawn` to set your town spawn.

**Q: Can I change my nickname?**
A: Yes, if you're a VIP+ member! Use `/nick [name]`. Use `&` codes for colors.

**Q: What does mana do?**
A: Mana is used by special abilities in AuraSkills when you level up!

**Q: How do I join a nation?**
A: Your town mayor can add your town to a nation with `/nation add`.

---

## 📞 NEED HELP?

- Type `/help` to see all available commands
- Type `/rules` to read server rules
- Type `/motd` for server info
- Ask moderators in chat if you're stuck!
- Most commands have built-in help: try `/command ?`

**Enjoy your time on the server!** 🎮