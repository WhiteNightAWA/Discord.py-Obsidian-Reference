### is_ws_ratelimited () [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AutoShardedClient.is_ws_ratelimited)

[bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") : Whether the websocket is currently rate limited.

This can be useful to know when deciding whether you should query members using HTTP or via the gateway.

This implementation checks if any of the shards are rate limited. For more granular control, consider [ShardInfo.is_ws_ratelimited()](discord/Data%20Classes/ShardInfo/is_ws_ratelimited).

*New in version 1.6.*
