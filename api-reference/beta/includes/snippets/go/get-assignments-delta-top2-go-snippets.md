---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphconfig "github.com/microsoftgraph/msgraph-beta-sdk-go/education"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestTop := int32(2)

requestParameters := &graphconfig.EducationClasseItemAssignmentsDelta()RequestBuilderGetQueryParameters{
	Top: &requestTop,
}
configuration := &graphconfig.EducationClasseItemAssignmentsDelta()RequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Education().Classes().ByClasseId("educationClass-id").Assignments().Delta().Get(context.Background(), configuration)


```