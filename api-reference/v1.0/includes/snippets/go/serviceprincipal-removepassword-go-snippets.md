---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  "github.com/google/uuid"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/ServicePrincipals/Item/RemovePassword"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewRemovePasswordPostRequestBody()
keyId := uuid.MustParse("f0b0b335-1d71-4883-8f98-567911bfdca6")
requestBody.SetKeyId(&keyId) 

graphClient.ServicePrincipals().ByServicePrincipalId("servicePrincipal-id").RemovePassword().Post(context.Background(), requestBody, nil)


```