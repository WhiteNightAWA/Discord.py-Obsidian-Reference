### `await` clone(_\*_, *name=None*, *reason=None*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.clone)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Clones this channel. This creates a channel with the same properties as this channel.

You must have the [manage_channels](discord/Data%20Classes/Permissions/manage_channels) permission to do this.

*New in version 1.1.*

- **Parameters**

	-   **name** ( Optional\[ [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ] ) – The name of the new channel. If not provided, defaults to this channel name.
    
	-   **reason** ( Optional\[ [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ] ) – The reason for cloning this channel. Shows up on the audit log.
    

- **Raises**

	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have the proper permissions to create this channel.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – Creating the channel failed.
    

- **Returns**

	- The channel that was created.

- **Return type**

	- [abc.GuildChannel](discord/Abstract%20Base%20Classes/GuildChannel/GuildChannel)

