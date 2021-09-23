### GuildChannel[](https://discordpy.readthedocs.io/en/v1.7.3/api.html#guildchannel)

> `class` discord.abc.**GuildChannel**

**Attributes** | | **Methods**
:--- | ---: | :---
[category](discord/Abstract%20Base%20Classes/GuildChannel/category) | `async`  | [clone](discord/Abstract%20Base%20Classes/GuildChannel/clone)
[changed_roles](discord/Abstract%20Base%20Classes/GuildChannel/changed_roles) | `async` | [create_invite](discord/Abstract%20Base%20Classes/GuildChannel/create_invite)
[created_at](discord/Abstract%20Base%20Classes/GuildChannel/created_at) | `async` | [delete](discord/Abstract%20Base%20Classes/GuildChannel/delete)
[guild](discord/Abstract%20Base%20Classes/GuildChannel/guild) | `async` | [invites](discord/Abstract%20Base%20Classes/GuildChannel/invites)
[mention](discord/Abstract%20Base%20Classes/GuildChannel/mention) | `async` | [move](discord/Abstract%20Base%20Classes/GuildChannel/move)
[name](discord/Abstract%20Base%20Classes/GuildChannel/name) | `def` | [overwrites_for](discord/Abstract%20Base%20Classes/GuildChannel/overwrites_for)
[overwrites](discord/Abstract%20Base%20Classes/GuildChannel/overwrites) | `def` | [permissions_for](discord/Abstract%20Base%20Classes/GuildChannel/permissions_for)
[permissions_synced](discord/Abstract%20Base%20Classes/GuildChannel/permissions_synced) | `async` | [set_permissions](discord/Abstract%20Base%20Classes/GuildChannel/set_permissions)
[position](discord/Abstract%20Base%20Classes/GuildChannel/position) ||


An ABC that details the common operations on a Discord guild channel.

The following implement this ABC:

-   [TextChannel](discord/Discord%20Models/TextChannel/TextChannel)
    
-   [VoiceChannel](discord/Discord%20Models/VoiceChannel/VoiceChannel)
    
-   [CategoryChannel](discord/Discord%20Models/CategoryChannel/CategoryChannel)
    
-   [StageChannel](discord/Discord%20Models/StageChannel/StageChannel)
    

This ABC must also implement [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake).

