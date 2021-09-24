### after [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.AuditLogChanges.after)

The new value. The attribute has the type of [AuditLogDiff](discord/Audit%20Log%20Data/AuditLogDiff/AuditLogDiff).

Depending on the [AuditLogActionCategory](discord/Enumerations/AuditLogActionCategory) retrieved by [category](discord/Audit%20Log%20Data/AuditLogEntry/category), the data retrieved by this attribute differs:

Category | Description
--- | ---
[create](discord/Enumerations/AuditLogActionCategory#create) | All attributes are set to the created value
[delete](discord/Enumerations/AuditLogActionCategory#delete) |  attributes are set to `None` 
[update](discord/Enumerations/AuditLogActionCategory#update) |  attributes are set the value after updating. 
`None` | No attributes are set.

