## roles [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.AllowedMentions.roles)
Controls the roles being mentioned. 
If `True` (the default) then roles are mentioned based on the message content. 
If `False` then roles are not mentioned at all. 
If a list of [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) is given then only the roles provided will be mentioned, provided those roles are in the message content.

- **Type**
	- Union[ [bool](https://docs.python.org/3/library/functions.html#bool), List[ [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) ] ]

