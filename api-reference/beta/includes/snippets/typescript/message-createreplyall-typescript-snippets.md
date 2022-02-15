---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.message = new Message();
requestBody.message.attachments = [
				new Attachment();
requestBody.message.attachments.additionalData = new Map([
						["@odata.type", "#microsoft.graph.fileAttachment"];
						["name", "guidelines.txt"];
						["contentBytes", "bWFjIGFuZCBjaGVlc2UgdG9kYXk="];
					]);
			]
		],
requestBody.comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.";
const result = async () => {
	await graphServiceClient.me.messagesById("message-id").createReplyAll.post(requestBody);
}


```