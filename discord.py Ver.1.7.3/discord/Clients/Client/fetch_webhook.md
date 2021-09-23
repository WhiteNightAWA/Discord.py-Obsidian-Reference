### `await` fetch_webhook [](https://discordpy.readthedocs.io/en/v1.7.3/api.html#discord.Client.fetch_webhook)

This function is a [coroutine](https://docs.python.org/3/library/asyncio-task.html#coroutine).

Retrieves a [Webhook](discord/Webhook%20Support/Webhook/Webhook) with the specified ID.


- **Raises**

	- [HTTPException](discord/Exceptions/HTTPException) – Retrieving the webhook failed.

	- [NotFound](discord/Exceptions/NotFound) – Invalid webhook ID.

	- [Forbidden](discord/Exceptions/Forbidden) – You do not have permission to fetch this webhook.

- **Returns**

	- The webhook you requested.

- **Return type**

	- [Webhook](discord/Webhook%20Support/Webhook/Webhook)




