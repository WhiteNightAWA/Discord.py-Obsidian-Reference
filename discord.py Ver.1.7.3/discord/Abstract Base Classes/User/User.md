## User [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#user)
> `class` discord.abc.User

**Attributes**|
:---|
[avatar](discord/Abstract%20Base%20Classes/User/avatar)|
[bot](discord/Abstract%20Base%20Classes/User/bot)|
[discriminator](discord/Abstract%20Base%20Classes/User/discriminator)|
[display_name](discord/Abstract%20Base%20Classes/User/display_name)|
[mention](discord/Abstract%20Base%20Classes/User/mention)|
[name](discord/Abstract%20Base%20Classes/User/name)|
An ABC that details the common operations on a Discord user.

The following implement this ABC:

- [User](discord/Discord%20Models/User/User)

- [ClientUser](discord/Discord%20Models/ClientUser/ClientUser)

- [Member](discord/Discord%20Models/Member/Member)

This ABC must also implement [Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake).


