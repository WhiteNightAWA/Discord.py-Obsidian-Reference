### `await` change_presence (_\*_, *activity=None*, *status=None*, *afk=False*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.change_presence)
This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Changes the client’s presence.

Example:
```python
game = discord.Game("with the API")
await client.change_presence(status=discord.Status.idle, activity=game)
```

- **Parameters**

	- **activity** (Optional[ [BaseActivity](discord/Data%20Classes/BaseActivity/BaseActivity) ]) - The activity being done. `None` if no currently active activity is done.
	- **status** (Optional[ [Status](discord/Enumerations/Status) ]) - Indicates what status to change to. If `None`, then [Status.online](discord/Enumerations/Status#online) is used.

	- **afk** (Optional[ [bool](https://docs.python.org/3/library/functions.html#bool) ]) - Indicates if you are going AFK. This allows the discord client to know how to handle push notifications better for you in case you are actually idle and not lying.

- **Raises**

	- [**InvalidArgument**](discord/Exceptions/InvalidArgument) – If the activity parameter is not the proper type.

