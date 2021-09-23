### `await` fetch_widget[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_widget)

This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Gets a [Widget](discord/Discord%20Models/Widget/Widget) from a guild ID.

> #### Note
> The guild must have the widget enabled to get this information.

- **Parameters**

	- **guild_id** ( [int](https://docs.python.org/3/library/functions.html#int) ) – The ID of the guild.

- **Raises**
	- [Forbidden](discord/Exceptions/Forbidden) – The widget for this guild is disabled.

	- [HTTPException](discord/Exceptions/HTTPException) – Retrieving the widget failed.

- **Returns**

	- The guild’s widget.

- **Return type**

	- [Widget](discord/Discord%20Models/Widget/Widget)

