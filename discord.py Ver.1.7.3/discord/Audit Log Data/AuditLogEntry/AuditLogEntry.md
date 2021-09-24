## AuditLogEntry [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#auditlogentry)
Represents an Audit Log entry.
You retrieve these via [Guild.audit_logs()](discord/Discord%20Models/Guild/audit_logs).
> #### Supported Operations
> **x == y**
> Checks if two entries are equal.
> **x != y**
> Checks if two entries are not equal.
> **hash(x)**
> Returns the entry’s hash.

*Changed in version 1.7: Audit log entries are now comparable and hashable.*
****
> `class` discord.**AuditLogEntry**(_\*_, *users*, *data*, *guild*)

Attributes|
:---|
[action](discord/Audit%20Log%20Data/AuditLogEntry/action) |
[after](discord/Audit%20Log%20Data/AuditLogEntry/after) |
[before](discord/Audit%20Log%20Data/AuditLogEntry/before) |
[category](discord/Audit%20Log%20Data/AuditLogEntry/category) |
[changes](discord/Audit%20Log%20Data/AuditLogEntry/changes) |
[created_at](discord/Audit%20Log%20Data/AuditLogEntry/created_at) |
[extra](discord/Audit%20Log%20Data/AuditLogEntry/extra) |
[id](discord/Audit%20Log%20Data/AuditLogEntry/id) |
[reason](discord/Audit%20Log%20Data/AuditLogEntry/reason) |
[target](discord/Audit%20Log%20Data/AuditLogEntry/target) |
[user](discord/Audit%20Log%20Data/AuditLogEntry/user) |

