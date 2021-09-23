### `await` set\_permissions (*target*, _\*_, *overwrite=see - below*, *reason=None*, _\*\*permissions_) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.set_permissions "Permalink to this definition")

This function is a [_coroutine_](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Sets the channel specific permission overwrites for a target in the channel.

The `target` parameter should either be a [Member](discord/Discord%20Models/Member/Member) or a [Role](discord/Discord%20Models/Role/Role) that belongs to guild.

The `overwrite` parameter, if given, must either be `None` or [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite). For convenience, you can pass in keyword arguments denoting [Permissions](discord/Data%20Classes/Permissions/Permissions) attributes. If this is done, then you cannot mix the keyword arguments with the `overwrite` parameter.

If the `overwrite` parameter is `None`, then the permission overwrites are deleted.

You must have the `manage_roles` permission to use this.

Examples:

Setting allow and deny:
```python
await message.channel.set_permissions(message.author, read_messages=True, send_messages=False)
```
Deleting overwrites:
```python
await channel.set_permissions(member, overwrite=None)
```
Using [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite) :
```python
overwrite = discord.PermissionOverwrite()
overwrite.send_messages = False
overwrite.read_messages = True
await channel.set_permissions(member, overwrite=overwrite)
```

- **Parameters**

	-   **target** ( Union\[ [Member](discord/Discord%20Models/Member/Member), [Role](discord/Discord%20Models/Role/Role) ] ) – The member or role to overwrite permissions for.
    
	-   **overwrite** ( Optional\[ [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite) ] ) – The permissions to allow and deny to the target, or `None` to delete the overwrite.
    
	-   **\*\*permissions** – A keyword argument list of permissions to set for ease of use. Cannot be mixed with `overwrite`.
    
	-   **reason** ( Optional\[ [str](https://docs.python.org/3/library/stdtypes.html#str "(in Python v3.9)") ] ) – The reason for doing this action. Shows up on the audit log.
    

- **Raises**

	-   [**Forbidden**](discord/Exceptions/Forbidden) – You do not have permissions to edit channel specific permissions.
    
	-   [**HTTPException**](discord/Exceptions/HTTPException) – Editing channel specific permissions failed.
    
	-   [**NotFound**](discord/Exceptions/NotFound) – The role or member being edited is not part of the guild.
    
	-   [**InvalidArgument**](discord/Exceptions/InvalidArgument) – The overwrite parameter invalid or the target type was not [Role](discord/Discord%20Models/Role/Role) or [Member](discord/Discord%20Models/Member/Member).

