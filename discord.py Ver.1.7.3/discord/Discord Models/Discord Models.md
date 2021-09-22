# Discord Models [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord-models)
Models are classes that are received from Discord and are not meant to be created by the user of the library.
****

> ## Danger
> The classes listed below are **not intended to be created by users** and are also **read-only**.
>
> For example, this means that you should not make your own [User](./User/User) instances nor should you modify the [User](./User/User) instance yourself.
>
> If you want to get one of these model classes instances they'd have to be through the cachet and a common way of doing so is through the [utils.find](discord/Utility%20Functions/find) function or attributes of model classes that you receive from the events specified in the [Event Reference](discord/Event%20Reference/Event%20Reference).

> ## Note
> 
> Nearly all classes here have [\__slots__](https://docs.python.org/3/reference/datamodel.html#slots) defined which means that it is impossible to have dynamic attributes to the data classes.
****

- [ClientUser](./ClientUser/ClientUser)
- [[Relationship]](./Relationship/Relationship)
- [User](./User/User)
- [Attachment](./Attachment/Attachment)
- [Asset](./Asset/Asset)
- [Message](./Message/Message)
- [DeletedReferencedMessage](./DeletedReferencedMessage/DeletedReferencedMessage)
- [Reaction](./Reaction/Reaction)
- [CallMessage](./CallMessage/CallMessage)
- [GroupCall](./GroupCall/GroupCall)
- [Guild](./Guild/Guild)
- [Integration](./Integration/Integration)
- [Member](./Member/Member)
- [Spotify](./Spotify/Spotify)
- [VoiceState](./VoiceState/VoiceState)
- [Emoji](./Emoji/Emoji)
- [PartialEmoji](./PartialEmoji/PartialEmoji)
- [Role](./Role/Role)
- [RoleTage](./RoleTage/RoleTage)
- [TextChannel](./TextChannel/TextChannel)
- [StoreChannel](./StoreChannel/StoreChannel)
- [VoiceChannel](./VoiceChannel/VoiceChannel)
- [StageChannel](./StageChannel/StageChannel)
- [CategoryChannel](./CategoryChannel/CategoryChannel)
- [DMChannel](./DMChannel/DMChannel)
- [GroupChannel](./GroupChannel/GroupChannel)
- [PartialInviteGuild](./PartialInviteGuild/PartialInviteGuild)
- [PartialInviteChannel](./PartialInviteChannel/PartialInviteChannel)
- [Invite](./Invite/Invite)
- [Template](./Template/Template)
- [WidgetChannel](./WidgetChannel/WidgetChannel)
- [WidgetMember](./WidgetMember/WidgetMember)
- [Widget](./Widget/Widget)
- [Sticker](./Sticker/Sticker)
- [RawMessageDeleteEvent](./RawMessageDeleteEvent/RawMessageDeleteEvent)
- [RawBulkMessageDeleteEvent](./RawBulkMessageDeleteEvent/RawBulkMessageDeleteEvent)
- [RawMessageUpdateEvent](./RawMessageUpdateEvent/RawMessageUpdateEvent)
- [RawReactionActionEvant](./RawReactionActionEvant/RawReactionActionEvant)
- [RawReactionClearEvent](./RawReactionClearEvent/RawReactionClearEvent)
- [RawReactionClearEmojiEvent](./RawReactionClearEmojiEvent/RawReactionClearEmojiEvent)






