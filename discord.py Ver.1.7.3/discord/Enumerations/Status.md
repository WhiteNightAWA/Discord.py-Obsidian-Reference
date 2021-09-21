## `class` discord.**Status** [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.Status)
Specifies a [Member](discord/Discord%20Models/Member/Member)'s status.
****
### online
The member is online.

### offline
The member is offline.

### idle
The member is idle.

### dnd
The member is “Do Not Disturb”.

### do_not_disturb
An alias for [dnd](#dnd).

### invisible
The member is “invisible”. In reality, this is only used in sending a presence a la [Client.change_presence()](discord/Clients/Client/change_presence). 
When you receive a user’s presence this will be [offline](#offline) instead.

