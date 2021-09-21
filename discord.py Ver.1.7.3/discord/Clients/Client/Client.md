# Client [¶](https://discordpy.readthedocs.io/en/stable/api.html#client)
Represents a client connection that connects to Discord. This class is used to interact with the Discord WebSocket and API.

A number of options can be passed to the [Client](discord/Clients/Client/Client).

****
> `class` discord.**Client**(_*_, _loop=None_, _**options_)

**Attributes**||**Methods**
:---|---:|:--- |
[activity](./activity) | `async` | application_info
[allowed_mentions](./allowed_mentions) | `async` | before_identify_hook
cached_messages | `async` | [change_presence](./change_presence)
emojis | `def` | clear
guilds | `async` | close
intents | `async` | connect
latency | `async` | create_guild
loop | `async` | delete_invite
private_channels | `@` | event
user | `async` | fetch_channel
users | `async` | fetch_guild
voice_clients | `def` | fetch_guilds
ws | `async` | fetch_invite
| | `async` | fetch_template
| | `async` | fetch_user
| | `async` | fetch_user_profile
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
