### `await` send (*content=None*, \*, *tts=False*, *embed=None*, *file=None*, *files=None*, *delete_after=None*, *nonce=None*, *allowed\_mentions=None*, *reference=None*, *mention\_author=None*)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.Messageable.send)

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Sends a message to the destination with the content given.

The content must be a type that can convert to a string through `str(content)`. If the content is set to `None` (the default), then the `embed` parameter must be provided.

To upload a single file, the `file` parameter should be used with a single [File](discord/Data%20Classes/File/File) object. To upload multiple files, the `files` parameter should be used with a [list](https://docs.python.org/3/library/stdtypes.html#list "(in Python v3.9)") of [File](discord/Data%20Classes/File/File) objects. **Specifying both parameters will lead to an exception**.

If the `embed` parameter is provided, it must be of type [Embed](discord/Data%20Classes/Embed/Embed) and it must be a rich embed type.

- **Parameters**

	-   **content** ( [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ) – The content of the message to send.
    
	-   **tts** ( [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ) – Indicates if the message should be sent using text-to-speech.
    
	-   **embed** ( [Embed](discord/Data%20Classes/Embed/Embed) ) – The rich embed for the content.
    
	-   **file** ( [File](discord/Data%20Classes/File/File) ) – The file to upload.
    
	-   **files** ( List\[ [File](discord/Data%20Classes/File/File) ] ) – A list of files to upload. Must be a maximum of 10.
    
	-   **nonce** ( [int](https://docs.python.org/3/library/functions.html#int "(in Python v3.9)") ) – The nonce to use for sending this message. If the message was successfully sent, then the message will have a nonce with this value.
    
	-   **delete_after** ( [float](https://docs.python.org/3/library/functions.html#float "(in Python v3.9)") ) – If provided, the number of seconds to wait in the background before deleting the message we just sent. If the deletion fails, then it is silently ignored.
    
	-   **allowed_mentions** ( [AllowedMentions](discord/Data%20Classes/AllowedMentions/AllowedMentions) ) – Controls the mentions being processed in this message. If this is passed, then the object is merged with [allowed_mentions](discord/Clients/Client/allowed_mentions). The merging behaviour only overrides attributes that have been explicitly passed to the object, otherwise it uses the attributes set in [allowed_mentions](discord/Clients/Client/allowed_mentions). If no object is passed at all then the defaults given by [allowed_mentions](discord/Clients/Client/allowed_mentions) are used instead.
    
		*New in version 1.4.*
    
	-   **reference** ( Union\[ [Message](discord/Discord%20Models/Message/Message), [MessageReference](discord/Data%20Classes/MessageReference/MessageReference) ] ) – A reference to the [Message](discord/Discord%20Models/Message/Message) to which you are replying, this can be created using [to_reference()](discord/Discord%20Models/Message/to_reference) or passed directly as a [Message](discord/Discord%20Models/Message/Message). You can control whether this mentions the author of the referenced message using the [replied_user](discord/Data%20Classes/AllowedMentions/replied_user) attribute of `allowed_mentions` or by setting `mention_author`.
    
    	*New in version 1.6.*
    
	-   **mention_author** ( Optional\[ [bool](https://docs.python.org/3/library/functions.html#bool "(in Python v3.9)") ] ) – If set, overrides the [replied_user](discord/Data%20Classes/AllowedMentions/replied_user) attribute of `allowed_mentions`.
    
 	   *New in version 1.6.*
    

- **Raises**

	-   [**HTTPException**](discord/Exceptions/HTTPException) – Sending the message failed.
    
	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have the proper permissions to send the message.
    
	-   [**InvalidArgument**](discord/Exceptions/InvalidArgument) – The `files` list is not of the appropriate size, you specified both `file` and `files`, or the `reference` object is not a [Message](discord/Discord%20Models/Message/Message) or [MessageReference](discord/Data%20Classes/MessageReference/MessageReference).
    

- **Returns**

	- The message that was sent.

- **Return type**

	- [Message](discord/Discord%20Models/Message/Message)

