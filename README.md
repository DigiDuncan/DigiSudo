# DigiSudo
DigiSudo is a cog for discord.py bots that adds one command, `sudo`, which allows the command runner to run any other command the bot has a different user.

The command syntax is `sudo @user [command...]`.

By default, the command can only be run by either the owner of the bot (as in, the person who controls the bot's token) or all the members of the team that owns the bot. This restriction can be removed by ommiting the `@commands.is_owner()` check on line 15 of `sudo.py` if you are adding this file directly into your bot, though this is **not reccomended.** The restrcition currently can not be removed if you install the cog via `pip`.

The cog can be installed with:

`pip install git+git://github.com/DigiDuncan/DigiSudo.git`

Once it is installed, any discord.py can load it with:

`bot.load_extension("sudo")`
