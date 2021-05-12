# PokeHelper-Public
PokeHelper Issue Repository

This repository is meant for the tracking of issues and suggestions for PokeHelper Development.

Please see the issues section to log new issues:
https://github.com/Astelan5/PokeHelper-Public/issues

# PokeHelper Features:

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

## Goals

## Clan/Server
