
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.MailFolders["inbox"].MessageRules["AQAAAJ5dZp8="]
	.Request()
	.DeleteAsync();

```