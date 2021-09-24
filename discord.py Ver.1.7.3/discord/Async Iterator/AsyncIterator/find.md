### `await` find (*predicate*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AsyncIterator.find)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Similar to [utils.find()](discord/Utility%20Functions/find) except run over the async iterator.

Unlike [utils.find()](discord/Utility%20Functions/find), the predicate provided can be a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Getting the last audit log with a reason or `None`:
```python
def predicate(event):
    return event.reason is not None

event = await guild.audit_logs().find(predicate)
```
- **Parameters**

	- **predicate** – The predicate to use. Could be a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

- **Returns**

	- The first element that returns `True` for the predicate or `None`.

