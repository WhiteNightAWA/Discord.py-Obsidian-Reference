### `async with` typing () [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.Messageable.typing)

Returns a context manager that allows you to type for an indefinite period of time.

This is useful for denoting long computations in your bot.

> #### Note
> This is both a regular context manager and an async context manager. This means that both `with` and `async with` work with this.

Example Usage:
```python
async with channel.typing():
    # do expensive stuff here
    await channel.send('done!')
```
