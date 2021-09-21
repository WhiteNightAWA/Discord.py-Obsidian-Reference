# Exceptions [¶](https://discordpy.readthedocs.io/en/stable/api.html#exceptions)
The following exceptions are thrown by the library.


## Exception Hierarchy
****
- [Exceptions](./Exceptions)

	- [DiscordException](./DiscordException)

		- [ClientException](./ClientException)

			- [InvalidData](./InvalidData)

			- [InvalidArgument](./InvalidArgument)

			- [LoginFailure](./LoginFailure)

			- [ConnectionClosed(_socket_, _*_, _shard_id_, _code=None_)](./ConnectionClosed)

			- [PrivilegedIntentsRequired(_shard_id_)](./PrivilegedIntentsRequired)

		- [NoMoreItems](./NoMoreItems)

		- [GatewayNotFound](./GatewayNotFound)

		- [HTTPException(_response_, _message_)](./HTTPException)

			- [Forbidden(_response_, _message_)](./Forbidden)

			- [NotFound(_response_, _message_)](./NotFound)

			- [DiscordServerError(_response_, _message_)](./DiscordServerError)

- [opus.OpusError(_code_)](./opus.OpusError)

- [opus.OpusNotLoaded](./opus.OpusNotLoaded)


#errors 