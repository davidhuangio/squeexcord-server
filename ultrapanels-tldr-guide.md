# Restart Server

Press the restart button to restart the server. The server will automatically load into `de_dust2`

# Common Console Commands

The console panel is where you will issue **steamCMD** commands into the server. These commands are the same commands you would type into your local console i.e. `sv_cheats 1`

Some of the more common commands include: \
\
`changelevel <map_name>`<span data-text-color="gray"> - Used to change the server's map to a map installed into the server. This currently only works for the native de\_ maps like </span>`de_dust2` and not any workshop maps (for now).

`host_workshop_map <workshop_id>` - Used to change the server's map to a workshop map. If the server has already downloaded the map, the map will change immediately, otherwise it will take some time to download. (There doesn't seem to be any console logs to see this). You can find the workshop id by looking in the url of the workshop page.\
\
`sv_cheats 1` - used to turn on cheats, this is mostly for turning on noclip. \
\
`say` - used to send a console message to the server that the entire server can see, can be tough to see replies if game is going on in console (thinking of getting a plugin that sends chats to discord) 

`exec <gamemode_gametype>` - used to force the server to load a specific game mode's config. Right now the `!cs` runs `exec gamemode_competitive` while `!dm` runs `exec gamemode_deathmatch`. I removed the `!surf` command for now but if the map gets into surf and gets screwed up you can run `exec gamemode_surf` to force exec the surf config. \
\
`status` - prints to the console a list of players, the current map, etc. 

`banid <minutes> <userid>` - ban's userid (from status) for specified minutes. set minutes to `0` to ban indefinitely. i.e. `ban 0 123456`

`css_plugins list` - shows the currently loaded **CounterStrikeSharp** plugins. Good to debug if a new plugin is loaded or not. 

# MatchZy Admins

As MatchZy admins you can use these commands in-game to force certain events to happen. \
\
`.forcestart` - forces a match to start into knife round, use this when people aren't readying up (min 4 players atm)

`.restart` - forces the current match to restart to warmup

`.prac` - puts the game into practice mode

`.exitprac` - exits the game out of practice mode

`.pause` - pauses the current freezetime or next round's freezetime

<https://shobhit-pathak.github.io/MatchZy/commands/> - more commands/configs