
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = await graphClient.Groups["b320ee12-b1cd-4cca-b648-a437be61c5cd"]
	.Request()
	.Select( e => new {
			 e.AllowExternalSenders,
			 e.AutoSubscribeNewMembers,
			 e.IsSubscribedByMail,
			 e.UnseenCount 
			 })
	.GetAsync();

```