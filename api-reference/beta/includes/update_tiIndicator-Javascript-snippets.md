
```Javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const tiIndicator = {
  additionalInformation: "additionalInformation-after-update",
  confidence: 42,
  description: "description-after-update",
};

let res = await client.api('/security/tiIndicators/{id}')
	.version('beta')
	.update({tiIndicator : tiIndicator});

```