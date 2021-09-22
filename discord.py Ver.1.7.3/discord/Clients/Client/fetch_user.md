### `await` fetch_user (*user_id*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_user)
The function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Retrieves a [User](discord/Discord%20Models/User/User) based on their ID. This can only be used by bot accounts. You do not have to share any guilds with the user to get this information, however many operations do require that you do.

> #### Note
> This method is an API call. If you have [Intents.members](discord/Data%20Classes/Intents/members) and member cache enabled, consider [get_user()](./get_user) instead.

- **Parameters**

	- **user_id** ( [int](https://docs.python.org/3/library/functions.html#int) ) - The user's **ID** to fetch from.

- **Raises**

	- [NotFound](discord/Exceptions/NotFound) - A user with this **ID** does not exist.

	- [HTTPException](discord/Exceptions/HTTPException) - Fetching the user failed.

- **Returns**

	- The user you requested.

- **Return type**

	- [User](discord/Discord%20Models/User/User)

