### get_all_members () [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.get_all_members)

Returns a generator with every [Member](discord/Discord%20Models/MEmber/Member) the client can see.

This is equivalent to:

```python
for guild in client.guilds:
    for member in guild.members:
        yield member
```

- **Yields**

	- [Member](discord/Discord%20Models/MEmber/Member) - A member the client can see.

