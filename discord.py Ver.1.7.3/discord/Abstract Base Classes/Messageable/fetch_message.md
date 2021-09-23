### `await` fetch_message (*id*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.Messageable.fetch_message "Permalink to this definition")

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Retrieves a single [Message](discord/Discord%20Models/Message/message) from the destination.

This can only be used by bot accounts.

- **Parameters**

	- **id** ([int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)")) – The message ID to look for.

- **Raises**

	-   [**NotFound**](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.NotFound "discord.NotFound") – The specified message was not found.
    
	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have the permissions required to get a message.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – Retrieving the message failed.
    

- **Returns**

	- The message asked for.

- **Return type**

	- [Message](discord/Discord%20Models/Message/message)

