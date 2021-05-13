# PokeHelper-Public
PokeHelper Issue Repository

This repository is meant for the tracking of issues and suggestions for PokeHelper Development.

Please see the issues section to log new issues:
https://github.com/Astelan5/PokeHelper-Public/issues

# Quickstart

## Timers
To quickly enable all timers run `)timers on` and `)timers all on`.  
To remove the timer set messages run `)timers qm on`.  
To enable pings on timer completion run `)timers ping on`.  
  
To see your current timer settings run `)setting timers`.  
  
See `)help timers` for more information about configuring your timers.  
## Goals
To get started with goals run `)goal set <number>` and PokeHelper will begin tracking your progress. See `)help goal` for more goal options.
## Alerts
If you would like alerts for your catchbot or quest run `)alert cb on` and `)alert quest on` respectively.  
To setup market alerts run `)alerts market <pokemon-name/dex-number>`. To set a price threshold run `)alerts market price <price>`.  
To setup remaining ball alerts run `)alerts ball on`. To set a ball threshold run `)alerts ball th <number>`.  
## General
See `)help` for all available commands and `)help <command>` for more information about a specific command.  
  
**Use the command `)init user` to see this message in discord.**

# PokeHelper Features:

## Fishing
PokeHelper displays the rarity of pokemon when fishing.  
![Image of Fishing Message No Embed](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/General/fishing_no_embed.PNG?raw=true)  

`)toggle embeds fish On`:  
  
![Image of Fishing Message Embed](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/General/fishing_embed.PNG?raw=true)  

## Rare Spawn Notifications:  
PokeHelper will ping you and send out information when you find a rare pokemon.  
![Image of Rare Info Embed Off](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/General/Rare%20Spawns/Rare_message_no_embed_new_format.PNG?raw=true)  
  
`)toggle embeds On`:  

![Image of Rare Info Embed On](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/General/Rare%20Spawns/Rare_message_embed_new_format.PNG?raw=true)  
# Commands

## General
- `donate` :  
Provides a link to donate to the creator.
- `flute` :  
displays the last seen flute message with a calculated countdown till golden hour.  
![Image of flute command](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/flute_command.PNG?raw=true)  
- `invite` :  
Provides a link to invite PokeHelper to a new server.
- `search` :  
Allows you to search for a pokemon in the PokeHelper database by `name` or `dex number`.
- `settings` :  
aliases: `set`, `setting`  
Displays settings based on the argument provided.
  - `user` :  
  Command: `)settings user`  
  aliases: `u`  
  Displays your current user settings.
  - `timers`  
  Command: `)settings timers`  
  aliases: `ti`, `timer`  
  Displays your current timer settings.
  - `alerts` :  
  Command: `)settings alerts`  
  aliases: `alert`  
  Displays your current alert settings.
  - `clan` :  
  Command: `)settings clan`  
  aliases: `c`  
  Displays your current clan/server settings.
- `swaptracker` :  
usage: `)swaptracker <session-label> <number-of-swap-to-track>`  
optional arguments: `<current-swap-multiplier>` `<swaps-today>`
Running this command begins a swap tracking session which will have the label `<session-label>` and last for `<number-of-swap-to-track>` swaps.  
  
  if you provide the two optional arguments after the two required ones PokeHelper will calculate and display your current swap multiplier as you swap. Alternatively if you open  the `;swap` page PokeHelper will automatically grab the two optional arguments and you will not need to enter them.  
  
  The two optional arguments must be used together. `<current-multiplier>` is your current multiplier from the `;swap` screen in `%` form. (if your Multiplier says `1.00x` enter `0`, if it says `+1%` enter `1`). `<swaps-today>` is the number in the Your swaps today row in the `;swap`
- `waterstate` :  
Displays the last seen waterstate.

## Settings
- `initialize` :  
aliases: `init`
  - `user` :  
  Initializes your user profile with PokeHelper and displays a quickstart guide.  
  Usage: `)init user`
  - `clan` :  
  Initializes your clan's (server) profile with PokeHelper.  
  Usage: `)init clan`
### Alerts
Use `)alerts` to activate this command. This command requires one of the options to be used.

aliases `alert`

**options:**
- `ball` :  
  Alerts users when they use their last ball of any type through a mention message. Sends the alert again each time they catch something until they purchase more. (only for catching not fishing at the moment) Activate using `)alert ball`. Takes the argument `On` or `Off`.  
  - `threshold` :  
  Sets a threshold other than the default `0` to trigger the alerts on. This applies to every type of ball. Activate using `)alert ball threshold`. Takes a numerical argument.  
![Image of ball alert](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Alerts/ball_alert.PNG?raw=true)
- `catchbot` :  
  Alerts the user in when their catchbot has returned and is ready to collect through a mention message. Activate using `)alert catchbot`. Takes the argument `On` or `Off`.  
![Image of catchbot alert](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Alerts/catchbot_alert.PNG?raw=true)
- `quest` :  
  Alerts the user when their next quest is available to pick up through a mention message. Activate using `)alert quest`. Takes the argument `On` or `Off`.  
![Image of quest alert](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Alerts/quest_alert.PNG?raw=true)
- `market` :  
  Sends a discord embed with information about the subscribed pokemon when a listing is detected and is either lower than the lowest know market price or lower than the price set by `)alert market price`. Activate using `)alert market`. Takes an argument of a `name` or `dex number` of a pokemon.
  - `price` :  
    Sets a price threshold to activate the market alert on. Activate using `)alert market price`. Takes a numerical argument.
![Image of market alert](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Alerts/market_alert.PNG?raw=true)

### Timers
Command: `)timers`

aliases: `ti`, `timer`

options:  
- `off/on` :  
  Command: `)timers on` or `)timers off`  
  options: `On` or `Off`  
  Toggles the timer functionality on or off.  
- `ping` :  
Command: `)timers ping`  
options: `On` or `Off`  
If `On` PokeHelper will mention the user in the timer complete message.
- `quietmode` :  
Command: `)timers quietmode` aliases: `qm`  
options: `On` or `Off`  
If `On` PokeHelper will not send the timer set message.
- `react` :  
Command: `)timers react`  
options: `On` or `Off`  
If `On` PokeHelper will react to the corresponding Pokemeow message when the timer is done instead of sending a message. Only works for Catch and Egg.  

__timers:__  
**The options for all timers is `On` or `Off`. The command for all timers is `)timers <timer-name>`**
- `all` :  
toggles all individual timers `On` or `Off`.  
- `battle`
- `box`
- `catch`
- `catchbot`
- `dex`
- `egg`
- `fish`
- `market`
- `open`
- `quest`
- `release`
- `shop`
- `swap`
- `team`

### Other Settings
`toggle` :  
aliases: `tog`  
**options:**  
- `embeds` :  
With embeds `On`:  
![Image of Embeds On](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/General/Rare%20Spawns/Rare_message_simple_embed.PNG?raw=true)  
With embeds `Off`:  
![Image of Embeds Off](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/General/Rare%20Spawns/rare_message_embed_off.PNG?raw=true)
- `embeds fish`
- `goal ping`
- `goal ping clan`
- `rare ping`
- `are ping spam`
- `rare message` :  
options: `On` or `Off`  
Setting this to `Off` disables the message that shows market values PokeHelper sends in your channel when you find a rare spawn.
- `rare spawn` :  
options: `Anonymous` or `Public`  
If set to `Anonymous` PokeHelper will not display your name or a message jump link in the server's rare spawn channel.

## Goals
`phgoal` :  
aliases: `goal`, `phg`  
**options**  
- `set` :  
Usage: `)phg set`  
argument: `<number>`  
Sets your personal catch goal to `<number>`. Does not reset your goal pinged status.
- `view` : 
Displays your progress towards your goal and your catch/encounter stats.  
![Image of Goal View](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Goals/goal_view.PNG?raw=true)
- `view clan` :  
Displays your progress towards your clan's goal.
- `reset` :  
Resets your tracked catches. **Does not effect stats**
- `extend` :  
Usage: `)phg extend`  
argument: `<number>`  
Increases your current goal by `<number>`. Resets your goal pinged status.
- `decrease` :  
Usage: `)phg decrease`  
argument: `<number>`  
Decreases your current goal by `<number>`. Resets your goal pinged status.
- `reset stats` :  
Resets your catch stats seen in the `)goal view` display.

## Clan/Server

### Clan

`leave_clan` :  
Prompts the user to leave their current PokeHelper clan.

`phclan` :  
aliases: `clan`, `phc`  
**options**  
- `add`
- `kick`
- `goal set`
- `goal view`
- `goal reset`
- `goal extend`
- `goal decrease`

### Server
`phserver` :  
aliases: `server`, `phs`  
**options**  
- `whitelist` :  
argument: `@role`  
Allows the mentioned role to activate any admin only PokeHelper commands such as those under `)phserver`  
- `blacklist` :  
argument: `@role`  
Stops the role from being able to activate any admin only PokeHelper commands such as those under `)phserver` 
- `prefix` :  
argument: `<anything>`
Changes the prefix for PokeHelper on your server to the provided text (no spaces).
- `golden channel` :  
argument : `#channel`  
Sets the mentioned channel up for golden hour pings. By default PokeHelper will ping the role `@Golden` unless changed with `)phs golden role`.  
![Image of golden ping](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Server/golden_ping.PNG?raw=true)  
- `golden role` :  
argument: `@role`  
Sets the mentioned role as the one to be pinged for golden hours in the golden channel.  
- `market channel` :  
arguments: `#channel` `[rarity]`  
PokeHelper will post market updates for the rarity specified to this channel. **Input <rarity> as all to apply this for all rarities. Input <channel> as disable to turn this off.**  
![Image of market update](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Server/pokehelper_market_update.PNG?raw=true)  
- `market role` :  
arguments: `@role` `[rarity]`  
PokeHelper will ping market updates for the rarity specified to this role.  
- `waterstate channel` :  
argument : `#channel`  
PokeHelper will post waterstate updates in this channel when it detects the waterstate has changed.  
**Input <channel> as disable to turn this off.**  
![Image of Waterstate update](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Server/waterstate_update.PNG?raw=true)
- `verify channel`  
- `rare channel` :  
argument : `#channel`  
Sets the given channel as the rare spawn channel where PokeHelper will post rare pokemon found in the server.
- `rare simple` :  
options: `On` or `Off`  
If `On` PokeHelper will display the simple version of rare spawns.  
![Image of Simple Rare Spawn](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Server/Simple_rare_spawn.PNG?raw=true)  
If `Off` PokeHelper will display the full version of rare spawns.  
![Image of Full Rare Spawn](https://github.com/Astelan5/PokeHelper-Public/blob/main/Pictures/Server/Full_rare_spawn.PNG?raw=true)
