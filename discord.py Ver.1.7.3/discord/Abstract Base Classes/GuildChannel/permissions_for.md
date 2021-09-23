### permissions_for (*member*)[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.abc.GuildChannel.permissions_for)

Handles permission resolution for the current [Member](discord/Discord%20Models/Member/Member).

This function takes into consideration the following cases:

-   Guild owner
-   Guild roles
-   Channel overrides
-   Member overrides
    

- **Parameters**

	- **member** ( [Member](discord/Discord%20Models/Member/Member) ) – The member to resolve permissions for.

- **Returns**

	- The resolved permissions for the member.

- **Return type**

	- [Permissions](discord/Data%20Classes/Permissions/Permissions)

