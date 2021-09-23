### `await` delete (_\*_, *reason=None*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.delete)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Deletes the channel.

You must have `manage_channels` permission to use this.

- **Parameters**

	- **reason** ( Optional\[ [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ] ) – The reason for deleting this channel. Shows up on the audit log.

- **Raises**

	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have proper permissions to delete the channel.
    
	-   [**NotFound**](discord/Exceptions/NotFound) – The channel was not found or was already deleted.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – Deleting the channel failed.

