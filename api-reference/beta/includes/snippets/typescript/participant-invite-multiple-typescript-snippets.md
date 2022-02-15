---
description: "Automatically generated file. DO NOT MODIFY"
---

```typescript

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
const graphServiceClient = new GraphServiceClient(requestAdapter);

const requestBody = new ()
requestBody.participants = [
			new InvitationParticipantInfo();
requestBody.participants.additionalData = new Map([
					["@odata.type", "#microsoft.graph.invitationParticipantInfo"];
					["replacesCallId", "a7ebfb2d-871e-419c-87af-27290b22e8db"];
						 ["@odata.type" , "#microsoft.graph.identitySet"],
							 ["@odata.type" , "#microsoft.graph.identity"],
							 ["id" , "7e1b4346-85a6-4bdd-abe3-d11c5d420efe"],
							 ["identityProvider" , "AAD"],
				]);
			new InvitationParticipantInfo();
requestBody.participants.additionalData = new Map([
					["@odata.type", "#microsoft.graph.invitationParticipantInfo"];
					["replacesCallId", "a7ebfb2d-871e-419c-87af-27290b22e8db"];
						 ["@odata.type" , "#microsoft.graph.identitySet"],
							 ["@odata.type" , "#microsoft.graph.identity"],
							 ["id" , "1e126418-44a0-4a94-a6f8-0efe1ad71acb"],
							 ["identityProvider" , "AAD"],
				]);
		]
	],
requestBody.clientContext = "f2fa86af-3c51-4bc2-8fc0-475452d9764f";
const result = async () => {
	await graphServiceClient.communications.callsById("call-id").participants.invite.post(requestBody);
}


```