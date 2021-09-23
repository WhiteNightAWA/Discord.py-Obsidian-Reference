### `await` invites ()[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.invites)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Returns a list of all active instant invites from this channel.

You must have `manage_channels` to get this information.

- **Raises**

	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have proper permissions to get the information.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – An error occurred while fetching the information.

- **Returns**

	- The list of invites that are currently active.

- **Return type**

	- List\[ [Invite](discord/Discord%20Models/Invite/Invite) ]

