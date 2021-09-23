### `await` connect(_\*_, *reconnect=True*)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AutoShardedClient.connect)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Creates a websocket connection and lets the websocket listen to messages from Discord. This is a loop that runs the entire event system and miscellaneous aspects of the library. Control is not resumed until the WebSocket connection is terminated.

- **Parameters**

	- **reconnect** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – If we should attempt reconnecting, either due to internet failure or a specific failure on Discord’s part. Certain disconnects that lead to bad state will not be handled (such as invalid sharding payloads or bad tokens).

- **Raises**

	- [**GatewayNotFound**](discord/Exceptions/GatewayNotFound) – If the gateway to connect to Discord is not found. Usually if this is thrown then there is a Discord API outage.
    
	- [**ConnectionClosed**](discord/Exceptions/GatewayNotFound) – The websocket connection has been terminated.

