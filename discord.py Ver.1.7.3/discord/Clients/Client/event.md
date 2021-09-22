### `@` event (*coro*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.event)
A decorator that registers an event to listen to.

You can find more info about the events on the [documentation below](discord/Event%20Reference/Event%20Reference).

The events must be a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine), if not, [TypeError](https://docs.python.org/3/library/exceptions.html#TypeError) is raised.

Example:
```python
@client.event
async def on_ready():
    print('Ready!')
```

- **Raises**

	- [TypeError](https://docs.python.org/3/library/exceptions.html#TypeError) - The coroutine passed is not actually a coroutine.

