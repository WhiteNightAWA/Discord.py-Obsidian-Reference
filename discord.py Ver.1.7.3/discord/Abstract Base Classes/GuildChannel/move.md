### `await` move (_\*\*kwargs_)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.move)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

A rich interface to help move a channel relative to other channels.

If exact position movement is required, `edit()` should be used instead.

You must have the [manage_channels](discord/Data%20Classes/Permissions/manage_channels) permission to do this.

> #### Note
> Voice channels will always be sorted below text channels. This is a Discord limitation.

*New in version 1.7.*

- **Parameters**

	-   **beginning** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Whether to move the channel to the beginning of the channel list (or category if given). This is mutually exclusive with `end`, `before`, and `after`.
    
	-   **end** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Whether to move the channel to the end of the channel list (or category if given). This is mutually exclusive with `beginning`, `before`, and `after`.
    
	-   **before** ( [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) ) – The channel that should be before our current channel. This is mutually exclusive with `beginning`, `end`, and `after`.
    
	-   **after** ( [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) ) – The channel that should be after our current channel. This is mutually exclusive with `beginning`, `end`, and `before`.
    
	-   **offset** ( [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ) – The number of channels to offset the move by. For example, an offset of `2` with `beginning=True` would move it 2 after the beginning. A positive number moves it below while a negative number moves it above. Note that this number is relative and computed after the `beginning`, `end`, `before`, and `after` parameters.
    
	-   **category** ( Optional\[ [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) ] ) – The category to move this channel under. If `None` is given then it moves it out of the category. This parameter is ignored if moving a category channel.
    
	-   **sync_permissions** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Whether to sync the permissions with the category (if given).
    
	-   **reason** ( [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ) – The reason for the move.
    

- **Raises**

	-   [**InvalidArgument**](discord/Exceptions/InvalidArgument) – An invalid position was given or a bad mix of arguments were passed.
    
	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have permissions to move the channel.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – Moving the channel failed.



