### `await` pins ()[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.Messageable.pins)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Retrieves all messages that are currently pinned in the channel.

> #### Note
> 
> Due to a limitation with the Discord API, the [Message](discord/Discord%20Models/Message/Message) objects returned by this method do not contain complete [Message.reactions](discord/Discord%20Models/Message/reactions) data.

- **Raises**

	- [**HTTPException**](discord/Exceptions/HTTPException) – Retrieving the pinned messages failed.

- **Returns**

	- The messages that are currently pinned.

- **Return type**

	- List[ [Message](discord/Discord%20Models/Message/Message) ]

