
```Cs

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var entityType = "Group";

var displayName = "Myprefix_test_mysuffix";

var mailNickname = "Myprefix_test_mysuffix";

var onBehalfOfUserId = "onBehalfOfUserId-value";

await graphClient.DirectoryObjects
	.ValidateProperties(entityType,displayName,mailNickname,onBehalfOfUserId)
	.Request()
	.PostAsync()

```