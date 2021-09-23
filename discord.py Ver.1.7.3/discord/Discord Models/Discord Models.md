# Discord Models [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord-models)
Models are classes that are received from Discord and are not meant to be created by the user of the library.
****

> ## Danger
> The classes listed below are **not intended to be created by users** and are also **read-only**.
>
> For example, this means that you should not make your own [User](discord/Discord%20Models/User/User) instances nor should you modify the [User](discord/Discord%20Models/User/User) instance yourself.
>
> If you want to get one of these model classes instances they'd have to be through the cachet and a common way of doing so is through the [utils.find](discord/Utility%20Functions/find) function or attributes of model classes that you receive from the events specified in the [Event Reference](discord/Event%20Reference/Event%20Reference).

> ## Note
> 
> Nearly all classes here have [\__slots__](https://docs.python.org/3/reference/datamodel.html#slots) defined which means that it is impossible to have dynamic attributes to the data classes.
****

- [ClientUser](discord/Discord%20Models/ClientUser/ClientUser)
- [[Relationship]](discord/Discord%20Models/Relationship/Relationship)
- [User](discord/Discord%20Models/User/User)
- [Attachment](discord/Discord%20Models/Attachment/Attachment)
- [Asset](discord/Discord%20Models/Asset/Asset)
- [Message](discord/Discord%20Models/Message/Message)
- [DeletedReferencedMessage](discord/Discord%20Models/DeletedReferencedMessage/DeletedReferencedMessage)
- [Reaction](discord/Discord%20Models/Reaction/Reaction)
- [CallMessage](discord/Discord%20Models/CallMessage/CallMessage)
- [GroupCall](discord/Discord%20Models/GroupCall/GroupCall)
- [Guild](discord/Discord%20Models/Guild/Guild)
- [Integration](discord/Discord%20Models/Integration/Integration)
- [Member](discord/Discord%20Models/Member/Member)
- [Spotify](discord/Discord%20Models/Spotify/Spotify)
- [VoiceState](discord/Discord%20Models/VoiceState/VoiceState)
- [Emoji](discord/Discord%20Models/Emoji/Emoji)
- [PartialEmoji](discord/Discord%20Models/PartialEmoji/PartialEmoji)
- [Role](discord/Discord%20Models/Role/Role)
- [RoleTage](discord/Discord%20Models/RoleTage/RoleTage)
- [TextChannel](discord/Discord%20Models/TextChannel/TextChannel)
- [StoreChannel](discord/Discord%20Models/StoreChannel/StoreChannel)
- [VoiceChannel](discord/Discord%20Models/VoiceChannel/VoiceChannel)
- [StageChannel](discord/Discord%20Models/StageChannel/StageChannel)
- [CategoryChannel](discord/Discord%20Models/CategoryChannel/CategoryChannel)
- [DMChannel](discord/Discord%20Models/DMChannel/DMChannel)
- [GroupChannel](discord/Discord%20Models/GroupChannel/GroupChannel)
- [PartialInviteGuild](discord/Discord%20Models/PartialInviteGuild/PartialInviteGuild)
- [PartialInviteChannel](discord/Discord%20Models/PartialInviteChannel/PartialInviteChannel)
- [Invite](discord/Discord%20Models/Invite/Invite)
- [Template](discord/Discord%20Models/Template/Template)
- [WidgetChannel](discord/Discord%20Models/WidgetChannel/WidgetChannel)
- [WidgetMember](discord/Discord%20Models/WidgetMember/WidgetMember)
- [Widget](discord/Discord%20Models/Widget/Widget)
- [Sticker](discord/Discord%20Models/Sticker/Sticker)
- [RawMessageDeleteEvent](discord/Discord%20Models/RawMessageDeleteEvent/RawMessageDeleteEvent)
- [RawBulkMessageDeleteEvent](discord/Discord%20Models/RawBulkMessageDeleteEvent/RawBulkMessageDeleteEvent)
- [RawMessageUpdateEvent](discord/Discord%20Models/RawMessageUpdateEvent/RawMessageUpdateEvent)
- [RawReactionActionEvant](discord/Discord%20Models/RawReactionActionEvant/RawReactionActionEvant)
- [RawReactionClearEvent](discord/Discord%20Models/RawReactionClearEvent/RawReactionClearEvent)
- [RawReactionClearEmojiEvent](discord/Discord%20Models/RawReactionClearEmojiEvent/RawReactionClearEmojiEvent)






