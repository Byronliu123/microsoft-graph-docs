---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.callbackUri = "https://bot.contoso.com/api/calls";
requestBody.acceptedModalities = [
			"audio";
		]
	],
requestBody.mediaConfig = new MediaConfig();
requestBody.mediaConfig.additionalData = new Map([
			["@odata.type", "#microsoft.graph.serviceHostedMediaConfig"];
			["preFetchMedia", [
						 ["uri" , "https://cdn.contoso.com/beep.wav"],
						 ["resourceId" , "1D6DE2D4-CD51-4309-8DAA-70768651088E"],
						 ["uri" , "https://cdn.contoso.com/cool.wav"],
						 ["resourceId" , "1D6DE2D4-CD51-4309-8DAA-70768651088F"],
				]
			],
		]);
async () => {
	await graphServiceClient.communications.callsById("call-id").answer.post(requestBody);
}


```