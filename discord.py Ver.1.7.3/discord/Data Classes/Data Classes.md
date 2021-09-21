# ## Data Classes [¶](https://discordpy.readthedocs.io/en/stable/api.html#data-classes)
Some classes are just there to be data containers, this lists them.

Unlike [models](discord/Discord%20Models/Discord%20Models) you are allowed to create most of these yourself, even if they can also be used to hold attributes.

Nearly all classes here have [__slots__](https://docs.python.org/3/reference/datamodel.html#slots) defined which means that it is impossible to have dynamic attributes to the data classes.

The only exception to this rule is[ abc.Snowflake](discord/Abstract%20Base%20Classes/Snowflake/Snowflake), which is made with dynamic attributes in mind.



