## Client [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#client)
Represents a client connection that connects to Discord. This class is used to interact with the Discord WebSocket and API.

A number of options can be passed to the [Client](discord/Clients/Client/Client).

****
> `class` discord.**Client**(_*_, _loop=None_, _**options_)

**Attributes**||**Methods**
:---|---:|:--- |
[activity](discord/Clients/Client/activity) | `async` | [application_info](discord/Clients/Client/application_info)
[allowed_mentions](discord/Clients/Client/allowed_mentions) | `async` | [before_identify_hook](discord/Clients/Client/before_identify_hook)
[cached_messages](discord/Clients/Client/cached_messages) | `async` | [change_presence](discord/Clients/Client/change_presence)
[emojis](discord/Clients/Client/emojis) | `def` | [clear](discord/Clients/Client/clear)
[guilds](discord/Clients/Client/guilds) | `async` | [close](discord/Clients/Client/close)
[intents](discord/Clients/Client/intents) | `async` | [connect](discord/Clients/Client/connect)
[latency](discord/Clients/Client/latency) | `async` | [create_guild](discord/Clients/Client/create_guild)
[loop](discord/Clients/Client/loop) | `async` | [delete_invite](discord/Clients/Client/delete_invite)
[private_channels](discord/Clients/Client/private_channels) | `@` | [event](discord/Clients/Client/event)
[user](discord/Clients/Client/user) | `async` | [fetch_channel](discord/Clients/Client/fetch_channel)
[users](discord/Clients/Client/users) | `async` | [fetch_guild](discord/Clients/Client/fetch_guild)
[voice_clients](discord/Clients/Client/voice_clients) | `def` | [fetch_guilds](discord/Clients/Client/fetch_guilds)
[ws](discord/Clients/Client/ws) | `async` | [fetch_invite](discord/Clients/Client/fetch_invite)
| | `async` | [fetch_template](discord/Clients/Client/fetch_template)
| | `async` | [fetch_user](discord/Clients/Client/fetch_user)
| | `async` | [fetch_user_profile](discord/Clients/Client/fetch_user_profile)
| | `async` | [fetch_webhook](discord/Clients/Client/fetch_webhook)
| | `async` | [fetch_widget](discord/Clients/Client/fetch_widget)
| | `def` | [get_all_channels](discord/Clients/Client/get_all_channels)
| | `def` | [get_all_members](discord/Clients/Client/get_all_members)
| | `def` | [get_channel](discord/Clients/Client/get_channel)
| | `def` | [get_emoji](discord/Clients/Client/get_emoji)
| | `def` | [get_guild](discord/Clients/Client/get_guild)
| | `def` | [get_user](discord/Clients/Client/get_user)
| | `def` | [is_closed](discord/Clients/Client/is_closed)
| | `def` | [is_ready](discord/Clients/Client/is_ready)
| | `def` | [is_ws_ratelimited](discord/Clients/Client/is_ws_ratelimited)
| | `async` | [login](discord/Clients/Client/login)
| | `async` | [logout](discord/Clients/Client/logout)
| | `async` | [on_error](discord/Clients/Client/on_error)
| | `async` | [request_offline_members](discord/Clients/Client/request_offline_members)
| | `def` | [run](discord/Clients/Client/run)
| | `async` | [start](discord/Clients/Client/start)
| | `async` | [wait_for](discord/Clients/Client/wait_for)
| | `async` | [wait_until_ready](discord/Clients/Client/wait_until_ready)
****
- **Parameters**

	- **max_messages** (Optional[ [int](https://docs.python.org/3/library/functions.html#int) ]) - The maximum number of messages to store in the internal message cache. This defaults to `1000`. Passing in `None` disables the message cache. 
	 
		 _Changed in version 1.3: Allow disabling the message cache and change the default size to `1000`._

	- **loop** ( Optional[ [asyncio.AbstractEventLoop](https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.AbstractEventLoop) ] ) - The [asyncio.AbstractEventLoop](https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.AbstractEventLoop) to use for asynchronous operations. Defaults to `None`, in which case the default event loop is used via [asyncio.get_event_loop()](https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.get_event_loop).

	- **connector** ( [aiohttp.BaseConnector](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.BaseConnector) ) - The connector to use for connection pooling.

	- **proxy** ( Optional[ [str](https://docs.python.org/3/library/stdtypes.html#str) ] ) - Proxy URL.

	- **proxy_auth** (	Optional[ [aiohttp.BasicAuth](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.BasicAuth) ] ) - An object that represents proxy HTTP Basic Authorization.

	- **shard_id** ( Optional[ [int](https://docs.python.org/3/library/functions.html#int) ] ) - Integer starting at `0` and less than [shard_count](discord/Data%20Classes/ShardInfo/shard_count).

	- **shard_count** ( Optional[ [int](https://docs.python.org/3/library/functions.html#int) ] ) - The total number of shards.

	- **intents** ( [Intents](discord/Data%20Classes/Intents/Intents) ) - The intents that you want to enable for the session. This is a way of disabling and enabling certain gateway events from triggering and being sent. If not given, defaults to a regularly constructed [Intents](discord/Data%20Classes/Intents/Intents) class.
	 
		_New in version 1.5._

	- **member_cache_flags** ( [MemberCacheFlags](discord/Data%20Classes/MemberCacheFlags/MemberCacheFlags) ) - Allows for finer control over how the library caches members. If not given, defaults to cache as much as possible with the currently selected intents.

		_New in version 1.5._

	- **fetch_offline_members** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - A deprecated alias of `chunk_guilds_at_startup`.

	- **chunk_guilds_at_startup** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - Indicates if [on_ready()](discord/Clients/Client/on_ready) should be delayed to chunk all guilds at start-up if necessary. This operation is incredibly slow for large amounts of guilds. The default is `True` if [Intents.members](discord/Data%20Classes/Intents/members) is `True`.

		_New in version 1.5._

	- **status** ( Optional[ [Status](discord/Enumerations/Status) ] ) - A status to start your presence with upon logging on to Discord.

	- **activity** ( Optional[ [BaseActivity](discord/Data%20Classes/BaseActivity/BaseActivity) ] ) - An activity to start your presence with upon logging on to Discord.

	- **allowed_mentions** ( Optional[ [AllowedMentions](discord/Data%20Classes/AllowedMentions/AllowedMentions) ] ) - Control how the client handles mentions by default on every message sent.

		_New in version 1.4._

	- **heartbeat_timeout** ( [float](https://docs.python.org/3/library/functions.html#float) ) - The maximum numbers of seconds before timing out and restarting the WebSocket in the case of not receiving a **HEARTBEAT_ACK**. Useful if processing the initial packets take too long to the point of disconnecting you. The default timeout is 60 seconds.

	- **guild_ready_timeout** ( [float](https://docs.python.org/3/library/functions.html#float) ) - The maximum number of seconds to wait for the **GUILD_CREATE** stream to end before preparing the member cache and firing **READY**. The default timeout is 2 seconds.

		_New in version 1.4._

	- **guild_subscriptions** ( [bool](https://docs.python.org/3/library/functions.html#float) ) - Whether to dispatch presence or typing events. Defaults to True.

		_New in version 1.3._

	- **assume_unsync_clock** ( [bool](https://docs.python.org/3/library/functions.html#bool) ) - Whether to assume the system clock is unsynced. This applies to the ratelimit handling code. If this is set to `True`, the default, then the library uses the time to reset a rate limit bucket given by Discord. If this is `False` then your system clock is used to calculate how long to sleep for. If this is set to `False` it is recommended to sync your system clock to Google’s NTP server.

		_New in version 1.3._

> ### Warning
> If this is set to `False` then the following features will be disabled:
> - No user related updates ( [on_user_update()](discord/Event%20Reference/on_user_update) will not dispatch )
> - All member related events will be disabled.
>	- [on_member_update()](discord/Event%20Reference/on_member_update)
>	- [on_member_join()](discord/Event%20Reference/on_member_join)
>	- [on_member_remove()](discord/Event%20Reference/on_member_remove)
> - Typing events will be disabled ( [on_typing()](discord/Event%20Reference/on_typing) ).
> - If `fetch_offline_members` is set to False then the user cache will not exist. This makes it difficult or impossible to do many things, for example:
> 	- Computing permissions
> 	- Querying members in a voice channel via [VoiceChannel.members](discord/Discord%20Models/VoiceChannel/members) will be empty.
> 	- Most forms of receiving [Member](discord/Discord%20Models/Member/Member) will be receiving [User](discord/Discord%20Models/User/User) instead, except for message events.
> 	- [Guild.owner](discord/Discord%20Models/Guild/owner) will usually resolve to `None`.
> 	- [Guild.get_member()](discord/Discord%20Models/Guild/get_member) will usually be unavailable.
> 	- Anything that involves using [Member](discord/Discord%20Models/Member/Member).
> 	- [users](discord/Clients/Client/users) will not be as populated.
> 	- etc.



