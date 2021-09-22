## `exception` discord.**ConnectionClosed**(_socket_, _*_, _shard_id_, _code=None_) [¶](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.ConnectionClosed)

Exception that’s thrown when the gateway connection is closed for reasons that could not be handled internally.

****

### code
The close code of the websocket.
- **Type**
	- [int](https://docs.python.org/3/library/functions.html#int)

### **reason**
The reason provided for the closure.
- **Type**
	- [str](https://docs.python.org/3/library/stdtypes.html#str)

### shard_id
The shard ID that got closed if applicable.
- **Type**
	- Optional[ [int](https://docs.python.org/3/library/functions.html#int) ]

#errors 