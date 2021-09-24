## AuditLogDiff [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#auditlogdiff)
Represents an audit log “change” object. A change object has dynamic attributes that depend on the type of action being done. Certain actions map to certain attributes being set.

Note that accessing an attribute that does not match the specified action will lead to an attribute error.

To get a list of attributes that have been set, you can iterate over them. To see a list of all possible attributes that could be set based on the action being done, check the documentation for [AuditLogAction](discord/Enumerations/AuditLogAction), otherwise check the documentation below for all attributes that are possible.
discord/Enumerations/AuditLogAction

> #### Supported Operations
> **iter(diff)**
> Returns an iterator over (attribute, value) tuple of this diff.

Attributes |
:--- |
[afk_channel](discord/Audit%20Log%20Data/AuditLogDiff/afk_channel)| 
[afk_timeout](discord/Audit%20Log%20Data/AuditLogDiff/afk_timeout) | 
[allow](discord/Audit%20Log%20Data/AuditLogDiff/allow) | 
[avatar](discord/Audit%20Log%20Data/AuditLogDiff/avatar) | 
[bitrate](discord/Audit%20Log%20Data/AuditLogDiff/bitrate) | 
[channel](discord/Audit%20Log%20Data/AuditLogDiff/channel) | 
[code](discord/Audit%20Log%20Data/AuditLogDiff/code) | 
[color](discord/Audit%20Log%20Data/AuditLogDiff/color) | 
[colour](discord/Audit%20Log%20Data/AuditLogDiff/colour) | 
[deaf](discord/Audit%20Log%20Data/AuditLogDiff/deaf) | 
[default_message_notifications](discord/Audit%20Log%20Data/AuditLogDiff/default_message_notifications) | 
[default_notifications](discord/Audit%20Log%20Data/AuditLogDiff/default_notifications) | 
[deny](discord/Audit%20Log%20Data/AuditLogDiff/deny) | 
[explicit_content_filter](discord/Audit%20Log%20Data/AuditLogDiff/explicit_content_filter) | 
[hoist](discord/Audit%20Log%20Data/AuditLogDiff/hoist) | 
[icon](discord/Audit%20Log%20Data/AuditLogDiff/icon) | 
[id](discord/Audit%20Log%20Data/AuditLogDiff/id) | 
[inviter](discord/Audit%20Log%20Data/AuditLogDiff/inviter) | 
[max_age](discord/Audit%20Log%20Data/AuditLogDiff/max_age) | 
[max_uses](discord/Audit%20Log%20Data/AuditLogDiff/max_uses) | 
[mentionable](discord/Audit%20Log%20Data/AuditLogDiff/mentionable) | 
[mfa_level](discord/Audit%20Log%20Data/AuditLogDiff/mfa_level) | 
[mute](discord/Audit%20Log%20Data/AuditLogDiff/mute) | 
[name](discord/Audit%20Log%20Data/AuditLogDiff/name) | 
[nick](discord/Audit%20Log%20Data/AuditLogDiff/nick) | 
[overwrites](discord/Audit%20Log%20Data/AuditLogDiff/overwrites) | 
[owner](discord/Audit%20Log%20Data/AuditLogDiff/owner) | 
[permissions](discord/Audit%20Log%20Data/AuditLogDiff/permissions) | 
[position](discord/Audit%20Log%20Data/AuditLogDiff/position) | 
[region](discord/Audit%20Log%20Data/AuditLogDiff/region) | 
[roles](discord/Audit%20Log%20Data/AuditLogDiff/roles) | 
[slowmode_delay](discord/Audit%20Log%20Data/AuditLogDiff/slowmode_delay) | 
[splash](discord/Audit%20Log%20Data/AuditLogDiff/splash) | 
[system_channel](discord/Audit%20Log%20Data/AuditLogDiff/system_channel) | 
[temporary](discord/Audit%20Log%20Data/AuditLogDiff/temporary) | 
[topic](discord/Audit%20Log%20Data/AuditLogDiff/topic) | 
[type](discord/Audit%20Log%20Data/AuditLogDiff/type) | 
[uses](discord/Audit%20Log%20Data/AuditLogDiff/uses) | 
[vanity_url_code](discord/Audit%20Log%20Data/AuditLogDiff/vanity_url_code) | 
[verification_level](discord/Audit%20Log%20Data/AuditLogDiff/verification_level) | 
[widget_channel](discord/Audit%20Log%20Data/AuditLogDiff/widget_channel) | 
[widget_enabled](discord/Audit%20Log%20Data/AuditLogDiff/widget_enabled) | 