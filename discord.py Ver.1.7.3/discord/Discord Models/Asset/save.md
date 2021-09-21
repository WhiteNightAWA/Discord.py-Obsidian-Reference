## `await` **save**(*fp*, _*_, *seek_begin=True*) [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.Asset.save)
This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Saves this asset into a file-like object.

- **Parameters**

	- **fp** (Union[ BinaryIO, [os.PathLike](https://docs.python.org/3/library/os.html#os.PathLike) ]) - Same as in [Attachment.save()](discord/Discord%20Models/Attachment/save)
	- **seek_begin** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - Same as in [Attachment.save()](discord/Discord%20Models/Attachment/save).

- **Raises**

	- [DiscordException](discord/Exceptions/DiscordException) – There was no valid URL or internal connection state.
	- [HTTPException](discord/Exceptions/HTTPException) – Downloading the asset failed.
	- [NotFound](discord/Exceptions/NotFound) – The asset was deleted.

- **Returns**

	- The number of bytes written.

- **Return type**

	- [int](https://docs.python.org/3/library/functions.html#int)

