### overwrites [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AuditLogDiff.overwrites)

A list of permission overwrite tuples that represents a target and a [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite) for said target.

The first element is the object being targeted, which can either be a [Member](discord/Discord%20Models/Member/member) or [User](discord/Discord%20Models/User/User) or [Role](discord/Discord%20Models/Role/Role). If this object is not found then it is a [Object](discord/Data%20Classes/Object/Object) with an ID being filled and a `type` attribute set to either `'role'` or `'member'` to help decide what type of ID it is.

- **Type**

	- List\[ Tuple\[ target, [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite) ] ]

