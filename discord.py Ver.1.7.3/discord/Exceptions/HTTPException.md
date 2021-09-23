## `exception` discord.**HTTPException**(_response_, _message_) [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.HTTPException)

Exception that’s thrown when an HTTP request operation fails.

***

### **response**

The response of the failed HTTP request. This is an instance of aiohttp.ClientResponse. In some cases this could also be a [requests.Response](http://docs.python-requests.org/en/latest/api/#requests.Response).

- **Type**
	-  [aiohttp.ClientResponse](https://docs.aiohttp.org/en/stable/client_reference.html#aiohttp.ClientResponse)

### **text**

The text of the error. Could be an empty string.

- **Type**
	- [str](https://docs.python.org/3/library/stdtypes.html#str)

### **status**

The status code of the HTTP request.

- **Type**
	- [int](https://docs.python.org/3/library/functions.html#int)

### **code**

The Discord specific error code for the failure.

- **Type**
	- [int](https://docs.python.org/3/library/functions.html#int)


#errors 