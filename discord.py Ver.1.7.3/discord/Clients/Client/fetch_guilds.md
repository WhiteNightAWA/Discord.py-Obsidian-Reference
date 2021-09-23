### `async for ... in` fetch_guilds (_\*_, *limit=100*, *before=None*, *after=None*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_guilds)
Retrieves an [AsyncIterator]() that enables receiving your guilds.

> #### Note
> Using this, you will only receive [Guild.owner](discord/Discord%20Models/Guild/owner) , [Guild.icon](discord/Discord%20Models/Guild/icon) , [Guild.id](discord/Discord%20Models/Guild/id) , and [Guild.name](discord/Discord%20Models/Guild/name) per [Guild](discord/Discord%20Models/Guild/Guild) .

> #### Note
> This method is an API call.
> For general usage, consider [guilds](discord/Clients/Client/guilds) instead.

Examples:

Usage:

```python
async for guild in client.fetch_guilds(limit=150):
    print(guild.name)
```

Flattening into a list:

```python
guilds = await client.fetch_guilds(limit=150).flatten()
# guilds is now a list of Guild...
```
All parameters are optional.

- **Parameters**

	- **limit** ( Optional[ [int](https://docs.python.org/3/library/functions.html#int) ] ) - The number of guilds to retrieve. If `None`, it retrieves every guild you have access to. Note, however, that this would make it a slow operation. Defaults to `100`.

	- **before** ( Union[ [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) , [date time.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) ] ) - Retrieves guilds before this date or object. If a date is provided it must be a timezone-naive datetime representing UTC time.

	- **after** ( Union[ [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) , [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime) ] ) - Retrieve guilds after this date or object. If a date is provided it must be a timezone-naive datetime representing UTC time.

- **Raises**

	- [HTTPException](discord/Exceptions/HTTPException) - Getting the guilds failed.

- **Yields**

	- [Guild](discord/Discord%20Models/Guild/Guild) - The guild with the guild data parsed.

