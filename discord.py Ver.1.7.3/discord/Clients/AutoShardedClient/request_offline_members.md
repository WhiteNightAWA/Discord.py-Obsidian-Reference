### `await` request_offline_members (_\*guilds_)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AutoShardedClient.request_offline_members)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Requests previously offline members from the guild to be filled up into the [Guild.members](discord/Discord%20Models/Guild/members) cache. This function is usually not called. It should only be used if you have the `fetch_offline_members` parameter set to `False`.

When the client logs on and connects to the websocket, Discord does not provide the library with offline members if the number of members in the guild is larger than 250. You can check if a guild is large if [Guild.large](discord/Discord%20Models/Guild/large) is `True`.

> #### Warning
>
> This method is deprecated. Use [Guild.chunk()](discord/Discord%20Models/Guild/chunk) instead.

- **Parameters**

	- **\*guilds** ( [Guild](discord/Discord%20Models/Guild/Guild) ) – An argument list of guilds to request offline members for.

- **Raises**

	- [**InvalidArgument**](discord/Exceptions/InvalidArgument) – If any guild is unavailable in the collection.

