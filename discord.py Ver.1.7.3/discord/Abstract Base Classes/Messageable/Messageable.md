## Messageable [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#messageable)

> `class` discord.abc.**Messageable**


||**Methods**
---:|:---
`async` | [fetch_message](discord/Abstract%20Base%20Classes/Messageable/fetch_message)
`def` | [history](discord/Abstract%20Base%20Classes/Messageable/history)
`async` | [pins](discord/Abstract%20Base%20Classes/Messageable/pins)
`async` | [send](discord/Abstract%20Base%20Classes/Messageable/send)
`async` | [trigger_typing](discord/Abstract%20Base%20Classes/Messageable/trigger_typing)
`def` | [typing](discord/Abstract%20Base%20Classes/Messageable/typing)

An ABC that details the common operations on a model that can send messages.

The following implement this ABC:

- [TextChannel](discord/Discord%20Models/TextChannel/TextChannel)

- [DMChannel](discord/Discord%20Models/DMChannel/DMChannel)

- [GroupChannel](discord/Discord%20Models/GroupChannel/GroupChannel)

- [User](discord/Discord%20Models/User/User)

- [Member](discord/Discord%20Models/Member/Member)

- [Context](discord.ext/Context/Context)

