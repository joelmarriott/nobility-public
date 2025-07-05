# Nobility Tribal Wars Discord Bot
Nobility is a Discord bot that provides various utilities to assist with 'Tribal Wars' the game founded by innogames.

## Contact
joel.marriott on discord

## Adding Nobility to Your Discord Server
Simply click the link below and select the server Nobility should join.  
_Note: You must have administrator permissions on the server to invite a bot_

https://discord.com/oauth2/authorize?client_id=960844255125991434&permissions=519232&integration_type=0&scope=bot+applications.commands

## Setting Up Nobility
1) Add Nobility to your server (above)
2) Set your global world (for the whole discord server) with the `/set_global_world` or `/sgw` command
3) Set individual channel worlds with the `/set_channel_world` or `/scw` command
4) That's it! You can now use any command listed below

## Commands
`/help` shows all possible commands in the discord interface
### World Settings
`/units` shows unit information for the current world  
`/world` shows setting information for the current world  
`/map` allows for custom maps to be generated for the current world  
_e.g._ `/map Tribe` shows the top 20 tribes  
_e.g._ `/map Player Player1,Player2 3` shows Player1 and Player2's conquers for the last 3 days  
_e.g._ `/map Player Player1,Player2 3 False False` is the same as above, but with all other player and barbarian villages removed.
### Player Information
`/player` shows information about player names containing your search string  
_e.g._ `/player tax` _would show player information for both 'Syntax' and 'Taxidermy'_  
_e.g._ `/player tax True` _would show full player information including OD for both 'Syntax' and 'Taxidermy'_  
`/villages` lists villages for a player (exact match, case insensitive)  
_e.g._ `/villages Syntax` _would show villages for 'Syntax' if they are a player on this world_
### Tribe Information
`/tribe` shows information about tribe names or tags (depending on search type) containing your search string  
_e.g._ `/tribe A1` _would show tribe information for the tags 'NA1' and 'A1N'_  
_e.g._ `/tribe warrior True Tribe Name` _would show full tribe information including OD for any tribes with names containing 'warrior'_
### Unit Calculations
`/distance` Shows the distance between two villages and the travel times to cover this distance for all units  
_e.g._ `/distance 111|111 222|222` will show the distance between the given villages  
`/backtime` can calculate the backtime of an attack given the origin, destination, landing time and unit speed  
_e.g._ `/backtime 111|111 222|222 Nobleman 12:30:56:314` will provide the backtime for this incoming noble