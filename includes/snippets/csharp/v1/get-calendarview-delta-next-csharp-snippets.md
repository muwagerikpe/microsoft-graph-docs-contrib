---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

// Code snippets are only available for the latest version. Current version is 5.x

var graphClient = new GraphServiceClient(requestAdapter);

var deltaRequestBuilder = new Microsoft.Graph.Me.CalendarView.Delta.DeltaRequestBuilder("https://graph.microsoft.com/v1.0/me/calendarView/delta?$deltatoken=R0usmcMDNGg0J1E", graphClient.RequestAdapter);
var result = await deltaRequestBuilder.GetAsync((requestConfiguration) =>
{
	requestConfiguration.Headers.Add("Prefer", "odata.maxpagesize=2");
});


```