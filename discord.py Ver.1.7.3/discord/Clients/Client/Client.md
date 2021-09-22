## Client [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#client)
Represents a client connection that connects to Discord. This class is used to interact with the Discord WebSocket and API.

A number of options can be passed to the [Client](discord/Clients/Client/Client).

****
> `class` discord.**Client**(_*_, _loop=None_, _**options_)

**Attributes**||**Methods**
:---|---:|:--- |
[activity](./activity) | `async` | [application_info](./application_info)
[allowed_mentions](./allowed_mentions) | `async` | [before_identify_hook](./before_identify_hook)
[cached_messages](./cached_messages) | `async` | [change_presence](./change_presence)
[emojis](./emojis) | `def` | [clear](./clear)
[guilds](./guilds) | `async` | [close](./close)
[intents](./intents) | `async` | [connect](./connect)
[latency](./latency) | `async` | [create_guild](./create_guild)
[loop](./loop) | `async` | [delete_invite](./delete_invite)
[private_channels](./private_channels) | `@` | [event](./event)
[user](./user) | `async` | [fetch_channel](./fetch_channel)
[users](./users) | `async` | [fetch_guild](./fetch_guild)
[voice_clients](./voice_clients) | `def` | [fetch_guilds](./fetch_guilds)
[ws](./ws) | `async` | [fetch_invite](./fetch_invite)
| | `async` | [fetch_template](./fetch_template)
| | `async` | [fetch_user](./fetch_user)
| | `async` | [fetch_user_profile](./fetch_user_profile)
| | `async` | fetch_webhook
| | `async` | fetch_widget
| | `def` | get_all_channels
| | `def` | get_all_members
| | `def` | get_channel
| | `def` | get_emoji
| | `def` | get_guild
| | `def` | get_user
| | `def` | is_closed
| | `def` | is_ready
| | `def` | is_ws_ratelimited
| | `async` | [login](./login)
| | `async` | logout
| | `async` | on_error
| | `async` | request_offline_members
| | `def` | run
| | `async` | start
| | `async` | wait_for
| | `async` | wait_until_ready
