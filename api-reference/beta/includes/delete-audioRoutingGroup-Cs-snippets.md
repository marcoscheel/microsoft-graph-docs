
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
	.Request()
	.DeleteAsync();

```