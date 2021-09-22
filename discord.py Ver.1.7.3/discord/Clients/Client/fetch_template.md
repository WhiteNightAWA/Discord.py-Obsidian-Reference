### `await` fetch_template (*code*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_template)
This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Gets a [Template](discord/Discord%20Models/Template/Template) from a [discord.new](https://discord.new) **URL** or code.

- **Parameters**

	- **code** ( Union[ [Template](discord/Discord%20Models/Template/Template) , [str](https://docs.python.org/3/library/stdtypes.html#str) ] )

- **Raises**

	- [NotFound](discord/Exceptions/NotFound) - The template is invalid.

	- [HTTPException](discord/Exceptions/HTTPException) - Getting the template failed.

- **Returns**

	- The template from the **URL**/code.

- **Return type**

	- [Template](discord/Discord%20Models/Template/Template)

