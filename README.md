# CensusPlus

A World of Warcraft addon that lets you survey and analyze your realm's player population in real-time.

## What is CensusPlus?

CensusPlus takes automatic snapshots of players on your realm by running targeted `/who` queries. It organizes the collected data by realm, faction, race, class, level, and guild—giving you detailed statistics about your server's population. Perfect for guild management, server analysis, or just curiosity about who plays on your realm.

## Features

- **Smart Census Scanning** — Automatically performs targeted `/who` queries to build a comprehensive player database
- **Flexible Filtering** — View players by guild, race, class, or level
- **Player List** — See detailed info about scanned characters (name, level, guild, last seen)
- **Minimap Button** — Quick access to census functions; draggable to any position around your minimap
- **Pause/Resume** — Pause a scan in progress without losing data
- **PVP Tracking** — Track honor kills and PVP statistics for players you inspect
- **Auto-Census** — Schedule automatic realm scans at configurable intervals
- **Data Management** — Export your collected data or prune old snapshots
- **Realm Detection** — Automatically detects US vs EU realms and localization

## Installation

1. Download and extract CensusPlus to your `World of Warcraft/Interface/AddOns/` directory
2. The addon will create a `CensusPlus` folder with all necessary files
3. Restart WoW and enable CensusPlus in your AddOns list
4. Type `/census` or click the minimap button to open the main window

## Quick Start

**Open CensusPlus:**
- Type `/census` or `/census+`
- Click the minimap button
- Or find it in your Addons menu

**Start Scanning:**
- Click the **Take** button to begin a census
- Optionally select filters (guild, race, class, level) before scanning
- The scan will run in the background—you can keep playing
- Minimize the window or hide the UI if you prefer

**View Results:**
- Open the Player List to see all scanned characters
- Filter by guild, race, class, or level to narrow results
- Right-click a player name for quick actions

## Commands

- `/census take` — Start a census scan
- `/census stop` — Stop the current scan
- `/census timer <minutes>` — Set auto-census interval
- `/census who <name>` — Search your local data for a player or guild
- `/census who unguilded <level>` — Find unguilded characters at a specific level
- `/census prune <days>` — Remove data older than X days
- `/census serverprune` — Keep only current server's data

## Options

Access settings via the main CensusPlus window or in your AddOns options panel:

- **Auto-Census** — Enable automatic scanning at set intervals
- **Show Minimap Button** — Toggle the minimap button visibility
- **Sound Alert** — Play a sound when a scan completes
- **Close Friends Panel** — Don't auto-open the Friends window during scans
- **Level Display** — Show level distribution as linear or logarithmic graph

## Data & Privacy

CensusPlus only collects data that's visible through standard `/who` queries—nothing more, nothing less. All data is stored locally on your computer.

## Tips

- Run multiple scans over time to track population trends
- Use filters to focus on specific guilds or level ranges
- Shift-click a player name while a scan is in progress to do a `/who` on them
- Paused scans preserve all collected data—resume whenever you want
- The player list caps at 1000 results per scan (plenty for most servers)

## Troubleshooting

**Scan won't start?**
- Census needs to be able to access `/who` results

**Getting "3 or fewer results" messages?**
- This is normal—it means that particular query had very few matches
- The addon will automatically divide and retry with narrower searches

**Data looks incomplete?**
- Larger realms take longer to fully scan; be patient
- Running multiple scans over time builds a more complete picture
- Use the prune function to clean up old data periodically

## License

CensusPlus is released under the GNU General Public License v2. See GPL.txt for details.

## Credits

Created by Ian Pieragostini
Modified By: Cooper Sellers (Rollie of Bloodscalp), Project Epoch Team, Bennylavaa
