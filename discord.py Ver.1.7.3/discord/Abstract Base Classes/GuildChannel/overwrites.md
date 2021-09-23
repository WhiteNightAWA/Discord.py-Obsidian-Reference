### overwrites [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.overwrites)

Returns all of the channel’s overwrites.

This is returned as a dictionary where the key contains the target which can be either a [Role](discord/Discord%20Models/Role/Role) or a [Member](discord/Discord%20Models/Member/Member) and the value is the overwrite as a [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite).

- **Returns**

	- The channel’s permission overwrites.

- **Return type**

	- Mapping\[ Union\[ [Role](discord/Discord%20Models/Role/Role), [Member](discord/Discord%20Models/Member/Member) ], [PermissionOverwrite](discord/Data%20Classes/PermissionOverwrite/PermissionOverwrite) ]

