### `await` read [](https://discordpy.readthedocs.io/en/stable/api.html#discord.Asset.read)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Retrieves the content of this asset as a [bytes](https://docs.python.org/3/library/stdtypes.html#bytes) object.

> **Warning**
> [PartialEmoji](discord/Discord%20Models/PartialEmoji/PartialEmoji) won’t have a connection state if user created, and a URL won’t be present if a custom image isn’t associated with the asset, e.g. a guild with no custom icon.

_New in version 1.1._

- **Raises**

	- [DiscordException](discord/Exceptions/DiscordException) – There was no valid URL or internal connection state.

	- [HTTPException](discord/Exceptions/HTTPException) – Downloading the asset failed.

	- [NotFound](discord/Exceptions/NotFound) – The asset was deleted.

- **Returns**

	- The content of the asset.

- **Return type**

	- [bytes](https://docs.python.org/3/library/stdtypes.html#bytes)
