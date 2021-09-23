### `await` fetch_channel (*channel_id*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_channel)
This function is a [coroutine](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel).

Retrieves a [abc.GuildChannel](discord/Abstract%20Base%20Classes/GuildChannel/GuildChannel) or abc.PrivateChannel with the specified ID.

> ### Note
> This method is an API call. For general usage, consider [get_channel()](discord/Clients/Client/get_channel) instead.

_New in version 1.2._

- **Raises**

	- [InvalidData](discord/Exceptions/InvalidData) - An unknown channel type was received form Discortd.

	- [HTTPException](discord/Exceptions/HTTPException) - Retrieving the channel failed.

	- [NotFound](discord/Exceptions/NotFound) - Invalid Channel ID.

	- [Forbidden](discord/Exceptions/Forbidden) - You do not have permission to fetch this channel.

- **Retruns**

	- The channel from the ID.

- **Return type**

	- Union[ [abc.GuildChannel](discord/Abstract%20Base%20Classes/GuildChannel/GuildChannel) , [abc.PrivateChannel](discord/Abstract%20Base%20Classes/PrivateChannel/PrivateChannel) ]



