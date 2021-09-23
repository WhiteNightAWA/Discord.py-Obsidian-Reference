### `await` fetch_guild (*guild_id*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_guild)
This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Retrieves a [Guild](discord/Discord%20Models/Guild/Guild) from an ID.

> ### Note
> Using this, you will **not** receive [Guild.channels](discord/Discord%20Models/Guild/channels) , [Guild.members](discord/Discord%20Models/Guild/members), [Member.activity](discord/Discord%20Models/Member/activity) and [Member.voice](discord/Discord%20Models/Member/voice) per [Member](discord/Discord%20Models/Member/Member)

> ### Note
> This method is an API call.
> For general usage, consider [get_guild()](discord/Clients/Client/get_guild) instead.

- **Parameters**

	- **guild_id** ( [int](https://docs.python.org/3/library/functions.html#int) ) - The guild's ID to fetch from.

- **Raises**

	- [Forbidden](discord/Exceptions/Forbidden) - You do not have access to the guild.

	- [HTTPException](discord/Exceptions/HTTPException) - Getting the guild failed

- **Returns**

	- The guild groom the ID.

- **Return type**

	- [Guild](discord/Discord%20Models/Guild/Guild)

