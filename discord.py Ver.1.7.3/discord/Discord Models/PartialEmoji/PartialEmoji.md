## PartialEmoji [](https://discordpy.readthedocs.io/en/stable/api.html#partialemoji)
****
> `class` discord.**PartialEmoji**

**Attributes** | | **Methods**
:--- | ---: | :---
[animated](./animated) | `def` | [is_custom_emoji](./is_custom_emoji)
[created_at](./created_at) | `def` | [is_unicode_emoji](./is_unicode_emoji)
[id](./id) | `def` | [url_as](./url_as)
[name](./name) |
[url](./url) |

Represents a “partial” emoji.

This model will be given in two scenarios:

- “Raw” data events such as [on_raw_reaction_add()]()

- Custom emoji that the bot cannot see from e.g. [Message.reactions]()

> ### Support Operations
> 
> **x == y**
> Checks if two emoji are the same.
> 
> **x != y**
> Checks if two emoji are not the same.
> 
> **hash(x)**
> Return the emoji’s hash.
> 
> **str(x)**
> Returns the emoji rendered for discord.



