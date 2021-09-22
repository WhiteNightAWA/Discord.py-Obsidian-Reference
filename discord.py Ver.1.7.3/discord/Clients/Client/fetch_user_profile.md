### `await` fetch_user_profile (*user_id*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_user_profile)

This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Gets an arbitrary user’s profile.

_Deprecated since version 1.7._

> #### Note
> This can only be used by non-bot accounts.

- **Parameters**

	- **user_id** ( [int](https://docs.python.org/3/library/functions.html#int) ) – The ID of the user to fetch their profile for.

- **Raises**

	- [Forbidden](discord/Exceptions/Forbidden) – Not allowed to fetch profiles.

	- [HTTPException](discord/Exceptions/HTTPException) – Fetching the profile failed.

- **Returns**

	- The profile of the user.

- **Return type**

	- [Profile](discord/Profile/Profile)

