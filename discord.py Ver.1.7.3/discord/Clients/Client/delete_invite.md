### `await` delete_invite (*invite*) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.delete_invite)
This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Revokes an [Invite](discord/Discord%20Models/Invite/Invite), URL, or ID to an invite.
obsidian://open?

You must have the manage_channels permission in the associated guild to do this.

- **Parameters**

	- **invite** ( Union[ [Invite](discord/Discord%20Models/Invite/Invite) , [str](https://docs.python.org/3/library/stdtypes.html#str) ] ) - The invite to revoke.

- **Raises**

	- [Forbidden](discord/Exceptions/Forbidden) - You do not have permissions to revoke invites.

	- [NotFound](discord/Exceptions/NotFound) - The invite is invalid or expired.

	- [HTTPException](discord/Exceptions/HTTPException) - Revoking the invite failed.

