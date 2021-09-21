# BaseActivity [¶](https://discordpy.readthedocs.io/en/stable/api.html#baseactivity)
****
> `class` discord.**BaseActivity**(**kwargs)

Attributes| 
---| 
[create_at](./create_at) | 

The base activity that all user-settable activities inherit from. A user-settable activity is one that can be used in [Client.change_presence](discord/Clients/Client/change_presence).

The following types currently count as user-settable:
- [Activity](discord/Data%20Classes/Activity/Activity)
- Game
- Streaming
- CustomActivity

Note that although these types are considered user-settable by the library, Discord typically ignores certain combinations of activity depending on what is currently set. This behaviour may change in the future so there are no guarantees on whether Discord will actually let you set these types.

_New in version 1.3._
