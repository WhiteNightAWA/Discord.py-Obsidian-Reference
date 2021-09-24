### map (*func*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AsyncIterator.map)

This is similar to the built-in [map](https://docs.python.org/3/library/functions.html#map "(in Python v3.9)") function. Another [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator) is returned that executes the function on every element it is iterating over. This function can either be a regular function or a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Creating a content iterator:
```python
def transform(message):
    return message.content

async for content in channel.history().map(transform):
    message_length = len(content)
```
- **Parameters**

	- **func** – The function to call on every element. Could be a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

- **Return type**

	- [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator)

