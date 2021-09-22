## AllowedMentions [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#allowedmentions)
A class that represents what mentions are allowed in a message.

This class can be set during [Client](discord/Clients/Client/Client) initialisation to apply to every message sent. It can also be applied on a per message basis via [abc.Messageable.send()](discord/Abstract%20Base%20Classes/Messageable/send) for more fine-grained control.

****
> `classes` discord.**AllowedMentions**(_*_, _everyone=True_, _users=True_, _roles=True_, _replied_user=True_)

**Attributes** | | **Methods**
:--- | ---: | :---
[everyone](./everyone) | `cls` | [AllowedMentions.all](./AllowedMentions.all)
[replied_user](./replied_user) | `cls` | [AllowedMentions.none](./AllowedMentions.none)
[roles](./roles) | |
[users](./users) | |


