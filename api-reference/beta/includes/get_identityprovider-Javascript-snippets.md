
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityProviders/Amazon-OAuth')
	.version('beta')
	.get();

```