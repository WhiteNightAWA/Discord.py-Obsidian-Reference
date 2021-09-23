# Data Classes [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#data-classes)
Some classes are just there to be data containers, this lists them.

Unlike [models](discord/Discord%20Models/Discord%20Models) you are allowed to create most of these yourself, even if they can also be used to hold attributes.

Nearly all classes here have [__slots__](https://docs.python.org/3/reference/datamodel.html#slots) defined which means that it is impossible to have dynamic attributes to the data classes.

The only exception to this rule is [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake), which is made with dynamic attributes in mind.


****
- [Object](discord/Data%20Classes/Object/Object)
- [Embed](discord/Data%20Classes/Embed/Embed)
- [AllowedMentions](discord/Data%20Classes/AllowedMentions/AllowedMentions)
- [MessageReference](discord/Data%20Classes/MessageReference/MessageReference)
- [PartialMessage](discord/Data%20Classes/PartialMessage/PartialMessage)
- [Intents](discord/Data%20Classes/Intents/Intents)
- [MemberCacheFlags](discord/Data%20Classes/MemberCacheFlags/MemberCacheFlags)
- [File](discord/Data%20Classes/File/File)
- [Color](discord/Data%20Classes/Color/Color)
- [BaseActivity](discord/Data%20Classes/BaseActivity/BaseActivity)
- [Activity](discord/Data%20Classes/Activity/Activity)
- [Game](discord/Data%20Classes/Game/Game)
- [Streaming](discord/Data%20Classes/Streaming/Streaming)
- [CustomActivity](discord/Data%20Classes/CustomActivity/CustomActivity)
- [Permissions](discord/Data%20Classes/Permissions/Permissions)
- [PermissionOverwite](discord/Data%20Classes/PermissionOverwite/PermissionOverwite)
- [ShardInfo](discord/Data%20Classes/ShardInfo/ShardInfo)
- [SystemChannelFlags](discord/Data%20Classes/SystemChannelFlags/SystemChannelFlags)
- [MessageFlags](discord/Data%20Classes/MessageFlags/MessageFlags)
- [PublicUserFlags](discord/Data%20Classes/PublicUserFlags/PublicUserFlags)

