### `await` create\_invite (_\*_, *reason=None*, _\*\*fields_) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.create_invite)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Creates an instant invite from a text or voice channel.

You must have the `create_instant_invite` permission to do this.

- **Parameters**

	-   **max_age** ( [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ) – How long the invite should last in seconds. If it’s 0 then the invite doesn’t expire. Defaults to `0`.
    
	-   **max_uses** ( [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ) – How many uses the invite could be used for. If it’s 0 then there are unlimited uses. Defaults to `0`.
    
	-   **temporary** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Denotes that the invite grants temporary membership (i.e. they get kicked after they disconnect). Defaults to `False`.
    
	-   **unique** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Indicates if a unique invite URL should be created. Defaults to True. If this is set to `False` then it will return a previously created invite.
    
	-   **reason** ( Optional\[ [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ] ) – The reason for creating this invite. Shows up on the audit log.
    

- **Raises**

	-   [**HTTPException**](discord/Exceptions/HTTPException) – Invite creation failed.
    
	-   [**NotFound**](discord/Exceptions/NotFound) – The channel that was passed is a category or an invalid channel.
    

- **Returns**

	- The invite that was created.

- **Return type**

	- [Invite](discord/Discord%20Models/Invite/Invite)

