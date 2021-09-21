## `exception` discord.**PrivilegedIntentsRequired**(_shard_id_) [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.PrivilegedIntentsRequired)
Exception that’s thrown when the gateway is requesting privileged intents but they’re not ticked in the developer page yet.

Go to https://discord.com/developers/applications/ and enable the intents that are required. Currently these are as follows:
- Intents.members

- Intents.presences

****

### shard_id
The shard ID that got closed if applicable.

- **Type**
	- Optional[ [int](https://docs.python.org/3/library/functions.html#int) ]


#errors 