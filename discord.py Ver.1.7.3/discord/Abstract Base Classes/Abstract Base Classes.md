# Abstract Base Classes []()
An [abstract base class](https://docs.python.org/3/glossary.html#term-abstract-base-class) (also known as an `abc`) is a class that models can inherit to get their behaviour. The Python implementation of an [abc](https://docs.python.org/3/library/abc.html) is slightly different in that you can register them at run-time. Abstract base classes cannot be instantiated. They are mainly there for usage with [isinstance()](https://docs.python.org/3/library/functions.html#isinstance) and [issubclass()](https://docs.python.org/3/library/functions.html#issubclass).

This library has a module related to abstract base classes, some of which are actually from the [abc](https://docs.python.org/3/library/abc.html) standard module, others which are not.
****
- [Snowflake](./Snowflake/Snowflake)
- [User](./User/User)
- [PrivateChannel](./PrivateChannel/PrivateChannel)
- [GuildChannel](./GuildChannel/GuildChannel)
- [Messageable](./Messageable/Messageable)
- [Connectable](./Connectable/Connectable)