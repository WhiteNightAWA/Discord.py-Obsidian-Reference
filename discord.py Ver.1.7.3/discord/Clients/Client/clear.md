### clear () [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.clear)
Clears the internal state of the bot.

After this, the bot can be considered “re-opened”, i.e. [is_closed()](discord/Clients/Client/is_closed) and [is_ready](discord/Clients/Client/is_ready) both return `False` along with the bot’s internal cache cleared.
