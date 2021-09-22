### `await` before_identify_hook (*shard_id*, _\*_, *initial=False*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.before_identify_hook)
This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

A hook that is called before IDENTIFYing a session. This is useful if you wish to have more control over the synchronization of multiple IDENTIFYing clients.

The default implementation sleeps for 5 seconds.

*New in version 1.4.*

- **Parameters**

	- **shard_id** ( [int](https://docs.python.org/3/library/functions.html#int) ) - The shard ID that requested being **IDENTIFY**’d

	- **initial** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - Whether this IDENTIFY is the first initial **IDENTIFY**.

