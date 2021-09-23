## AutoShardedClient []()
A client similar to [Client](discord/Clients/Client/Client) except it handles the complications of sharding for the user into a more manageable and transparent single process bot.

When using this client, you will be able to use it as-if it was a regular [Client](discord/Clients/Client/Client) with a single shard when implementation wise internally it is split up into multiple shards. This allows you to not have to deal with IPC or other complicated infrastructure.

It is recommended to use this client only if you have surpassed at least 1000 guilds.

If no [shard_count](discord/Data%20Classes/ShardInfo/shard_count) is provided, then the library will use the Bot Gateway endpoint call to figure out how many shards to use.

If a `shard_ids` parameter is given, then those shard IDs will be used to launch the internal shards. Note that [shard_count](discord/Data%20Classes/ShardInfo/shard_count) must be provided if this is used. By default, when omitted, the client will launch shards from 0 to `shard_count - 1`.

****
> `class` discord.**AutoShardedClient** (_*args_, *loop=None*, _**kwargs_)

**Attributes** | | **Methods**
:--- | ---: | :---
[latencies](discord/Clients/AutoShardedClient/latencies) | `async` | [change_presence](discord/Clients/AutoShardedClient/change_presence)
[latency](discord/Clients/AutoShardedClient/latency) | `async` | [close](discord/Clients/AutoShardedClient/close)
[shard_ids](discord/Clients/AutoShardedClient/shard_ids) | `async` | [connect](discord/Clients/AutoShardedClient/connect)
[shards](discord/Clients/AutoShardedClient/shards) | `def` | [get_shard](discord/Clients/AutoShardedClient/get_shard)
|| `def` | [is_ws_ratelimited](discord/Clients/AutoShardedClient/is_ws_ratelimited)
|| `async` | [request_offline_members](discord/Clients/AutoShardedClient/request_offline_members)

