### `async for ... in` history(_\*_, *limit=100*, *before=None*, *after=None*, *around=None*, *oldest_first=None*)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.Messageable.history)

Returns an [AsyncIterator](discord/Async%20Iterator/AsyncIterator/AsyncIterator) that enables receiving the destination’s message history.

You must have `read_message_history` permissions to use this.

Examples:

Usage:
```python
counter = 0
async for message in channel.history(limit=200):
    if message.author == client.user:
        counter += 1
```
Flattening into a list:
```python
messages = await channel.history(limit=123).flatten()
# messages is now a list of Message...
```

All parameters are optional.

- **Parameters**

	-   **limit** ( Optional[ [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ] ) – The number of messages to retrieve. If `None`, retrieves every message in the channel. Note, however, that this would make it a slow operation.
    
	-   **before** ( Optional\[ Union\[ [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) , [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime "(in Python v3.9)")] ] ) – Retrieve messages before this date or message. If a date is provided it must be a timezone-naive datetime representing UTC time.
    
	-   **after** ( Optional\[ Union\[ [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) , [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime "(in Python v3.9)")] ] ) – Retrieve messages after this date or message. If a date is provided it must be a timezone-naive datetime representing UTC time.
    
	-   **around** ( Optional\[ Union\[ [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) , [datetime.datetime](https://docs.python.org/3/library/datetime.html#datetime.datetime "(in Python v3.9)")] ] ) – Retrieve messages around this date or message. If a date is provided it must be a timezone-naive datetime representing UTC time. When using this argument, the maximum limit is 101. Note that if the limit is an even number then this will return at most limit + 1 messages.
    
	-   **oldest_first** ( Optional\[ [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ] ) – If set to `True`, return messages in oldest->newest order. Defaults to `True` if `after` is specified, otherwise `False`.
    

- **Raises**

	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have permissions to get channel message history.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – The request to get message history failed.
    

- **Yields**

	- [Message](discord/Discord%20Models/Message/Message) – The message with the message data parsed.

