---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = AddKeyPostRequestBody(
	key_credential = KeyCredential(
		type = "AsymmetricX509Cert",
		usage = "Verify",
		key = base64.urlsafe_b64decode("MIIDYDCCAki..."),
	),
	password_credential = None,
	proof = "eyJ0eXAiOiJ...",
)

result = await graph_client.applications.by_application_id('application-id').add_key.post(body = request_body)


```