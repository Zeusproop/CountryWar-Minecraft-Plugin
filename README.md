# CountryWar Minecraft Plugin

[![Modrinth](https://img.shields.io/badge/Modrinth-Available_Now-00AF5C?style=for-the-badge&logo=modrinth)](https://modrinth.com/plugin/countrywar)

**STILL IN VERY ALPHA** (Open issues here if you encounter any)

SharpnessMC inspired , a comprehensive team-based country war plugin for Minecraft servers. Features include dynamic health scaling for leaders, territory protection, supply drops, voting systems, and more!

## Features

### 1. Team & Leader Management
- **Dynamic Health Scaling**: Leaders get 20 hearts (double health)
- **Penalty Mechanics**: If a leader dies, teammates are set to 5 hearts
- **Automated Alliances**: Track friendly/hostile teams with scoreboard
- **Glowing Effect**: Remaining teammates glow when their leader dies

### 2. Economy & Loot Systems
- **Restricted World Interaction**: Mining and animal spawning disabled
- **Supply Drop System**: Tiered loot crates (Tier 1-3) with animations
- **Elimination Rewards**: Automatic bounty rewards ($1,000+)
- **Bounty System**: Place bounties on enemy teams

### 3. Area Buffs (Capital System)
- **Territory Protection**: Designated capital zones per team
- **Status Effects**: Regeneration and Speed buffs in own capital
- **Visual Indicators**: Boss bar notifications when entering territories
- **Damage Reduction**: 25% less damage when defending capital

### 4. Administrative Tools
- **Freeze Function**: Instantly freeze all 100 players for summits
- **Voting System**: GUI-based voting for bounties, alliances, wars
- **World Border Control**: Non-linear shrinks to specific regions
- **Punishment System**: Poison, glow, weakness, slowness, fines

### 5. Combat & Item Modification
- **Shield/Item Blacklisting**: Control item availability
- **Combat Tagging**: Prevent escape during combat
- **Friendly Fire Prevention**: No team damage


## Installation

1. Copy `CountryWar.jar` to your server's `plugins` folder
2. Restart your Minecraft server
3. Configure in `plugins/CountryWar/config.yml`

## Commands

### Admin Commands (`/cwadmin`)
| Command | Description |
|---------|-------------|
| `/cwadmin start` | Start the game |
| `/cwadmin stop` | End the game |
| `/cwadmin freeze` | Freeze all players |
| `/cwadmin unfreeze` | Unfreeze all players |
| `/cwadmin summit` | Call a leader summit |
| `/cwadmin createteam <name> <display>` | Create a team |
| `/cwadmin deleteteam <name>` | Delete a team |
| `/cwadmin addplayer <player> <team>` | Add player to team |
| `/cwadmin setleader <player>` | Set team leader |
| `/cwadmin setcapital <team> [radius]` | Set team capital |
| `/cwadmin supplydrop [tier]` | Spawn supply drop |
| `/cwadmin border <action>` | Manage world border |
| `/cwadmin punish <team> <type>` | Punish a team |
| `/cwadmin enableshields` | Enable shields in drops |
| `/cwadmin teams` | List all teams |

### Team Commands (`/team`)
| Command | Description |
|---------|-------------|
| `/team` | View your team info |
| `/team info <team>` | View team info |
| `/team list` | List all teams |
| `/team members` | List team members |
| `/team chat <msg>` | Team chat |
| `/team balance` | View team balance |
| `/team ally <team>` | Request alliance (Leader) |
| `/team enemy <team>` | Declare enemy (Leader) |

### Vote Commands (`/vote`)
| Command | Description |
|---------|-------------|
| `/vote yes` | Vote yes |
| `/vote no` | Vote no |
| `/vote status` | View vote status |
| `/vote menu` | Open voting GUI |
| `/vote start <type> <team>` | Start a vote |

### Bounty Commands (`/bounty`)
| Command | Description |
|---------|-------------|
| `/bounty` | List all bounties |
| `/bounty place <team> <amount>` | Place a bounty |
| `/bounty check <team>` | Check bounty on team |

## Configuration

See `config.yml` for all configuration options including:
- Game settings (mining, building, capital protection)
- Supply drop intervals and shield availability
- Economy rewards
- Leader health values
- Combat settings
- Voting parameters
- World border presets

## Permissions

| Permission | Description | Default |
|------------|-------------|---------|
| `countrywar.admin` | Admin commands | OP |
| `countrywar.player` | Player commands | true |

## Requirements

- Minecraft 1.20.x
- Spigot, Paper, or compatible server
- Java 17+

## License

NO License - All Rights Reserved.
