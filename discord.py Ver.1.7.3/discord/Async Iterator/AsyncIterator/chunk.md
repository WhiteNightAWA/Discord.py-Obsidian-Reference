### chunk (*max\_size*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AsyncIterator.chunk)

Collects items into chunks of up to a given maximum size. Another [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator) is returned which collects items into [list](https://docs.python.org/3/library/stdtypes.html#list "(in Python v3.9)")s of a given size. The maximum chunk size must be a positive integer.

*New in version 1.6.*

Collecting groups of users:
```python
async for leader, *users in reaction.users().chunk(3):
    ...
```
> #### Warning
> The last chunk collected may not be as large as `max_size`.

- **Parameters**

	- **max_size** – The size of individual chunks.

- **Return type**

	- [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator)

