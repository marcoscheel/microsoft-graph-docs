
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const calculate = {
  calculationType: "calculationType-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/application/calculate')
	.version('beta')
	.post(calculate);

```