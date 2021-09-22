### `await` create_guild (*name*, *region=None*, *icon=None*, _\*_, *code=None*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.create_guild)
This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Creates a [Guild](discord/Discord%20Models/Guild/Guild).

Bot accounts in more than 10 guilds are not allowed to create guilds.

- **Parameters**

	- **name** ( [str](https://docs.python.org/3/library/stdtypes.html#str) ) - The name of the guild.

	- **region** ( [VoiceRegion](discord/Enumerations/VoiceRegion) ) - The region for the voice communication server. Defaults to [VoiceRegion.us_west](discord/Enumerations/VoiceRegion#us_west).

	- **icon** ( [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) ) - The [bytes-like object](https://docs.python.org/3/glossary.html#term-bytes-like-object) representing the icon. See [ClientUser.edit()](discord/Discord%20Models/ClientUser/edit) for more details on what is expected.

	- **code** (.Optional[ [str](https://docs.python.org/3/library/stdtypes.html#str) ] ) - The code for a template to create the guild with.

		_New in version 1.4._

- **Raises**

	- [HTTPException](discord/Exceptions/HTTPException) - Guild creation failed.

	- [InvalidArgument](discord/Exceptions/InvalidArgument) - Invalid icon image format given. Must be PNG or JPG.

- **Returns**

	- The guild created. This is not the same guild that is added to cache.

- **Return type**

	- [Guild](discord/Discord%20Models/Guild/Guild)




		