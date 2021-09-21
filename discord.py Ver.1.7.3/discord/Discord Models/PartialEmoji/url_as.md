## url\_as(_*_, _format=None_, _static_format='png'_) [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.PartialEmoji.url_as)
Returns an [Asset](../Asset/Asset) for the emoji’s url, if it is custom.

The format must be one of ‘webp’, ‘jpeg’, ‘jpg’, ‘png’ or ‘gif’. ‘gif’ is only valid for animated emojis.

*New in version 1.7.*

- **Parameters**

	- **format** (Optional[ [str](https://docs.python.org/3/library/stdtypes.html#str) ]) - The format to attempt to convert the emojis to. If the format is `None`, then it is automatically detected as either ‘gif’ or static_format, depending on whether the emoji is animated or not.
	- **static_format** (Optional[ [str](https://docs.python.org/3/library/stdtypes.html#str) ]) - Format to attempt to convert only non-animated emoji’s to. Defaults to ‘png’
- **Raises**

	- [InvalidArgument](discord/Exceptions/InvalidArgument) – Bad image format passed to `format` or `static_format`.

- **Returns**

	- The resulting CDN asset.


- **Return type**
	- [Asset](../Asset/Asset)

