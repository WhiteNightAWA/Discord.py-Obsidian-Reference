# Async Iterator [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#async-iterator)
Some API functions return an “async iterator”. An async iterator is something that is capable of being used in an [async for statement](https://docs.python.org/3/reference/compound_stmts.html#async-for "(in Python v3.9)").

These async iterators can be used as follows:
```python
async for elem in channel.history():
    # do stuff with elem here
```
Certain utilities make working with async iterators easier, detailed below.
****
- ## [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator)

