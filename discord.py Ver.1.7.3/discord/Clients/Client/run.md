### run (_\*args_, _\*\*kwargs_) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.run)
A blocking call that abstracts away the event loop initialisation from you.

If you want more control over the event loop then this function should not be used. Use [start()](discord/Clients/Client/start) coroutine or [connect()](discord/Clients/Client/connect) + [login()](discord/Clients/Client/login).

Roughly Equivalent to:
```python
try:
    loop.run_until_complete(start(\*args, \*\*kwargs))
except KeyboardInterrupt:
    loop.run_until_complete(close())
    # cancel all tasks lingering
finally:
    loop.close()
```

> #### Warning
> This function must be the last function to call due to the fact that it is blocking. That means that registration of events or anything being called after this function call will not execute until it returns.

