---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = ListItemVersionRequestBuilder.ListItemVersionRequestBuilderGetQueryParameters(
		expand = ["fields"],
)

request_configuration = ListItemVersionRequestBuilder.ListItemVersionRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.sites.by_site_id('site-id').lists.by_list_id('list-id').items.by_item_id('listItem-id').versions.by_version_id('listItemVersion-id').get(request_configuration = request_configuration)


```