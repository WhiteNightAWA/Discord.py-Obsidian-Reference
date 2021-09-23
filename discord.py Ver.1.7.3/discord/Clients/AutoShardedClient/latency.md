### latency [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AutoShardedClient.latency)
Measures latency between a **HEARTBEAT** and a **HEARTBEAT_ACK** in seconds.

This operates similarly to [Client.latency()](discord/Clients/Client/latency) except it uses the average [latency](discord/Clients/AutoShardedClient/latency) of every shard’s latency. To get a list of shard latency, check the latencies property. Returns nan if there are no shards ready.

- **Type**

	- [float](https://docs.python.org/3/library/functions.html#float "(in Python v3.9)")

