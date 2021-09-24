### `await` get (_\*\*attrs_) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AsyncIterator.get)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Similar to [utils.get()](discord/Utility%20Functions/get) except run over the async iterator.

Getting the last message by a user named ‘Dave’ or `None`:
```python
msg = await channel.history().get(author__name='Dave')
```