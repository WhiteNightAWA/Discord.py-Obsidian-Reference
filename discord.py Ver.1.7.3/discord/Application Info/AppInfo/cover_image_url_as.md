### cover\_image\_url\_as (_\*_, *format='webp'*, *size=1024*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AppInfo.cover_image_url_as)

Returns an [Asset](discord/Discord%20Models/Asset/Asset) for the image on store embeds if this application is a game sold on Discord.

The format must be one of ‘webp’, ‘jpeg’, ‘jpg’ or ‘png’. The size must be a power of 2 between 16 and 4096.

*New in version 1.6.*

- **Parameters**

	-   **format** ( [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ) – The format to attempt to convert the image to. Defaults to ‘webp’.
    
	-   **size** ( [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ) – The size of the image to display.
    
- **Raises**

	- [**InvalidArgument**](discord/Exceptions/InvalidArgument) – Bad image format passed to `format` or invalid `size`.

- **Returns**

	- The resulting CDN asset.

- **Return type**

	- [Asset](discord/Discord%20Models/Asset/Asset)

