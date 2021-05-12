# PokeHelper-Public
PokeHelper Issue Repository

This repository is meant for the tracking of issues and suggestions for PokeHelper Development.

Please see the issues section to log new issues:
https://github.com/Astelan5/PokeHelper-Public/issues

# PokeHelper Features:

## General
- donate
- flute
- invite
- search
- settings
  - user
  - timers
  - alerts
  - clan
- swaptracker
- waterstate

## Settings
- initialize
### Alerts
Use `)alerts` to activate this command. This command requires one of the options to be used.

aliases `alert`

options:
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

timers: **The options for all timers is `On` or `Off`. The command for all timers is `)timers <timer-name>`**
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
