---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = ListRequestBuilder.ListRequestBuilderGetQueryParameters(
		select = ["name","lastModifiedDateTime"],
		expand = ["columns(select=name,description)","items",")"],
)

request_configuration = ListRequestBuilder.ListRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.sites.by_site_id('site-id').lists.by_list_id('list-id').get(request_configuration = request_configuration)


```