
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const mailFolder = {
  displayName: "displayName-value",
};

let res = await client.api('/me/mailFolders/{id}/childFolders')
	.version('beta')
	.post({mailFolder : mailFolder});

```