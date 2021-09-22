### `await` fetch\_invite (*url*, _\*_, *with_counts=True*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_invite)

This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Get an [Invite](discord/Discord%20Models/Invite/Invite) from a [discord.gg](https://discord.gg) **URL** or **ID**.

> #### Note
> If the invite is for a guild you have not joined, the guild and channel attributes of the returned [Invite](discord/Discord%20Models/Invite/Invite) will be [PartialInviteGuild](discord/Discord%20Models/PartialInviteGuild/PartialInviteGuild) and [PartialInviteChannel](discord/Discord%20Models/PartialInviteChannel/PartialInviteChannel) respectively.

- **Parameters**

	- **url** ( Union[ [Invite](discord/Discord%20Models/Invite/Invite) , [str](https://docs.python.org/3/library/stdtypes.html#str) ] ) - The Discord invite **ID** or **URL** (must be a discord.gg URL).

	- **with_counts** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - Whether to include count information in the invite. This fills the [Invite.approximate_member_count](discord/Discord%20Models/Invite/approximate_member_count) and [Invite.approximate_presence_count](discord/Discord%20Models/Invite/approximate_presence_count) fields.

- **Raises**

	- [NotFound](discord/Exceptions/NotFound) - THe invite has expired or is invalid.

	- [HTTPException](discord/Exceptions/HTTPException) - Getting the invite failed.

- **Returns**

	- The invite from the **URL**/**ID**.

- **Return type**

	- [Invite](discord/Discord%20Models/Invite/Invite)

