---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Security().Cases().EdiscoveryCases().ByEdiscoveryCaseId("ediscoveryCase-id").NoncustodialDataSources().ByNoncustodialDataSourceId("ediscoveryNoncustodialDataSource-id").MicrosoftGraphSecurityRelease().Post(context.Background(), nil)


```