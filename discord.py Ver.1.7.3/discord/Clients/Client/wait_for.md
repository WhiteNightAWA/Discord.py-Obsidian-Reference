### `await` wait_for (*event*, _\*_,* check=None*, *timeout=None*)
This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Waits for a WebSocket event to be dispatched.

This could be used to wait for a user to reply to a message, or to react to a message, or to edit a message in a self-contained way.

The `timeout` parameter is passed onto [asyncio.wait_for()](https://docs.python.org/3/library/asyncio-task.html#asyncio.wait_for "(in Python v3.9)"). By default, it does not timeout. Note that this does propagate the [asyncio.TimeoutError](https://docs.python.org/3/library/asyncio-exceptions.html#asyncio.TimeoutError "(in Python v3.9)") for you in case of timeout and is provided for ease of use.

In case the event returns multiple arguments, a [tuple](https://docs.python.org/3/library/stdtypes.html#tuple "(in Python v3.9)") containing those arguments is returned instead. Please check the [documentation](discord/Event%20Reference/Event%20Reference) for a list of events and their parameters.

This function returns the **first event that meets the requirements**.

Examples

Waiting for a user reply:

```python
@client.event
async def on_message(message):
    if message.content.startswith('$greet'):
        channel = message.channel
        await channel.send('Say hello!')

        def check(m):
            return m.content == 'hello' and m.channel == channel

        msg = await client.wait_for('message', check=check)
        await channel.send('Hello {.author}!'.format(msg))
```
Waiting for a thumbs up reaction from the message author:
```python
@client.event
async def on_message(message):
    if message.content.startswith('$thumb'):
        channel = message.channel
        await channel.send('Send me that 👍 reaction, mate')

        def check(reaction, user):
            return user == message.author and str(reaction.emoji) == '👍'

        try:
            reaction, user = await client.wait_for('reaction_add', timeout=60.0, check=check)
        except asyncio.TimeoutError:
            await channel.send('👎')
        else:
            await channel.send('👍')
```

- **Parameters**

	- **event** ( [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ) - The event name, similar to the [event reference](discord/Event%20Reference/Event%20Reference), but without the `on_` prefix, to wait for.

	- **check** ( Optional[ Callable[ …, [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ] ] ) - A predicate to check what to wait for. The arguments must meet the parameters of the event being waited for.

	- **timeout** ( Optional[ [float](https://docs.python.org/3/library/functions.html#float)  "(in Python v3.9)"] ) - The number of seconds to wait before timing out and raising [asyncio.TimeoutError](https://docs.python.org/3/library/asyncio-exceptions.html#asyncio.TimeoutError "(in Python v3.9)").

- **Raises**

	- [**asyncio.TimeoutError**](https://docs.python.org/3/library/asyncio-exceptions.html#asyncio.TimeoutError "(in Python v3.9)") - If a timeout is provided and it was reached.

- **Returns**

	- Returns no arguments, a single argument, or a [tuple](https://docs.python.org/3/library/stdtypes.html#tuple "(in Python v3.9)") of multiple arguments that mirrors the parameters passed in the [event reference](discord/Event%20Reference/Event%20Reference).

- **Return type**

	- Any
