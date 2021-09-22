### `await` login (*token*, _\*_, *bot=True*) [](https://discordpy.readthedocs.io/en/stable/api.html#discord.Client.login)

This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Logs in the client with the specified credentials.

This function can be used in two different ways.

> **Warning**
> Logging on with a user token is against the Discord [Terms of Service](https://support.discord.com/hc/en-us/articles/115002192352) and doing so might potentially get your account banned. Use this at your own risk.

- **Parameters**

	- **token** ( [str](https://docs.python.org/3/library/stdtypes.html#str) ) - The authentication token. Do not prefix this token with anything as the library will do it for you.

	- **bot** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - Keyword argument that specifies if the account logging on is a bot token or not.
  _Deprecated since version 1.7._
  
- **Raises**

	- [LoginFailure](discord/Exceptions/LoginFailure) - The wrong credentials are passed.

	- [HTTPException](discord/Exceptions/HTTPException) - An unknown HTTP related error occurred, usually when it isn’t 200 or the known incorrect credentials passing status code.

