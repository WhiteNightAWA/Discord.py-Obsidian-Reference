### filter (*predicate*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AsyncIterator.filter)

This is similar to the built-in [filter](https://docs.python.org/3/library/functions.html#filter "(in Python v3.9)") function. Another [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator) is returned that filters over the original async iterator. This predicate can be a regular function or a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Getting messages by non-bot accounts:
```python
def predicate(message):
    return not message.author.bot

async for elem in channel.history().filter(predicate):
    ...
```
- **Parameters**

	- **predicate** – The predicate to call on every element. Could be a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

- **Return type**

	- [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator)

