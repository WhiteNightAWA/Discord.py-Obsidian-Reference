## users [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.AllowedMentions.users)
Controls the users being mentioned. 
If `True` (the default) then users are mentioned based on the message content. 
If `False` then users are not mentioned at all. 
If a list of [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) is given then only the users provided will be mentioned, provided those users are in the message content.

- **Type**
	- Union[ [bool](https://docs.python.org/3/library/functions.html#bool), List[ [abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake) ] ]

