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
Use `)alerts` to activate this command.

aliases `alert`

options:
- `ball` :  
  Alerts users when they use their last ball of any type through a mention message. Sends the alert again each time they catch something until they purchase more. (only for catching not fishing at the moment) Activate using `)alert ball`. Takes the argument `On` or `Off`.  
  - `threshold` :  
  Sets a threshold other than the default `0` to trigger the alerts on. This applies to every type of ball. Activate using `)alert ball threshold`. Takes a numerical argument.
- `catchbot` :  
  Alerts the user in when their catchbot has returned and is ready to collect through a mention message. Activate using `)alert catchbot`. Takes the argument `On` or `Off`.
- `quest` :  
  Alerts the user when their next quest is available to pick up through a mention message. Activate using `)alert quest`. Takes the argument `On` or `Off`.
- `market` :  
  Sends a discord embed with information about the subscribed pokemon when a listing is detected and is either lower than the lowest know market price or lower than the price set by `)alert market price`. Activate using `)alert market`. Takes an argument of a `name` or `dex number` of a pokemon.
  - `price` :  
    Sets a price threshold to activate the market alert on. Activate using `)alert market price`. Takes a numerical argument.

### Timers

### Other Settings

## Goals

## Clan/Server
