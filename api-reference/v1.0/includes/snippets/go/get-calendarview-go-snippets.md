---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)


requestStartDateTime := "2017-01-01T19:00:00-08:00"
requestEndDateTime := "2017-01-07T19:00:00-08:00"

requestParameters := &graphconfig.CalendarViewRequestBuilderGetQueryParameters{
	StartDateTime: &requestStartDateTime,
	EndDateTime: &requestEndDateTime,
}
configuration := &graphconfig.CalendarViewRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.Me().Calendar().CalendarView().GetWithRequestConfigurationAndResponseHandler(configuration, nil)


```