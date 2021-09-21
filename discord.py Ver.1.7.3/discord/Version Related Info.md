## Version Related Info
****
There are two main ways to query version information about the library. For guarantees, check [Version Guarantees](https://discordpy.readthedocs.io/en/stable/version_guarantees.html#version-guarantees).

### discord.version_info [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.version_info)
A named tuple that is similar to [sys.version_info](https://docs.python.org/3/library/sys.html#sys.version_info).

Just like [sys.version_info](https://docs.python.org/3/library/sys.html#sys.version_info) the valid values for `releaselevel` are ‘alpha’, ‘beta’, ‘candidate’ and ‘final’.

### discord.__version__ [¶](https://discordpy.readthedocs.io/en/stable/api.html#discord.__version__)
A string representation of the version. e.g. `'1.0.0rc1'`. This is based off of [**PEP 440**](https://www.python.org/dev/peps/pep-0440).
