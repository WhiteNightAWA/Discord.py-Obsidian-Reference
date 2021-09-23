### `await` change\_presence(_\*_, *activity=None*, *status=None*, *afk=False*, *shard\_id=None*)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AutoShardedClient.change_presence)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Changes the client’s presence.

Example:

```python
game = discord.Game("with the API")
await client.change_presence(status=discord.Status.idle, activity=game)
```

- **Parameters**

	-   **activity** ( Optional[ [BaseActivity](discord/Data%20Classes/BaseActivity/BaseActivity) ] ) – The activity being done. `None` if no currently active activity is done.
    
	-   **status** ( Optional[ [Status](discord/Enumerations/Status) ] ) – Indicates what status to change to. If `None`, then [Status.online](discord/Enumerations/Status#online) is used.
    
	-   **afk** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Indicates if you are going AFK. This allows the discord client to know how to handle push notifications better for you in case you are actually idle and not lying.
    
	-   **shard_id** ( Optional[ [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ] ) – The shard_id to change the presence to. If not specified or `None`, then it will change the presence of every shard the bot can see.
    

- **Raises**

	- [**InvalidArgument**](discord/Exceptions/InvalidArgument) – If the `activity` parameter is not of proper type.

