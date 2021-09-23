### `for ... in` get_all_channels () [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.get_all_channels)

A generator that retrieves every [abc.GuildChannel](discord/Abstract%20Base%20Classes/GuildChannel/GuildChannel) the client can 'access'.

This is equivalent to:

```python
for guild in client.guilds:
    for channel in guild.channels:
        yield channel
```

> #### Note
> Just because you receive a [abc.GuildChannel](discord/Abstract%20Base%20Classes/GuildChannel/GuildChannel) does not mean that you can communicate in said channel. [abc.GuildChannel.permissions_for()](discord/Abstract%20Base%20Classes/GuildChannel/permissions_for) should be used for that.

- **Yields**

	- [abc.GuildChannel](discord/Abstract%20Base%20Classes/GuildChannel/GuildChannel) - A channel the client can 'access'.


