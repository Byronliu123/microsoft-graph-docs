---
title: "Update restrictedSignIn"
description: "Update the properties of a restrictedSignIn object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update restrictedSignIn
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [restrictedSignIn](../resources/restrictedsignin.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /auditLogs/restrictedSignIns/{restrictedSignInId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [restrictedSignIn](../resources/restrictedsignin.md) object.

The following table shows the properties that are required when you update the [restrictedSignIn](../resources/restrictedsignin.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|alternateSignInName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationMethodsUsed|String collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationProcessingDetails|[keyValue](../resources/intune-keyvalue.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationRequirement|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|clientAppUsed|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|conditionalAccessStatus|conditionalAccessStatus|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`.|
|correlationId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|flaggedForReview|Boolean|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|homeTenantId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|isInteractive|Boolean|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|ipAddress|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|ipAddressFromResourceProvider|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|mfaDetail|[mfaDetail](../resources/mfadetail.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|originalRequestId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|processingTimeInMilliseconds|Int32|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskEventTypes|riskEventType collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskEventTypes_v2|String collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|riskLevelAggregated|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|resourceDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|resourceId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|resourceTenantId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|servicePrincipalId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|servicePrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|signInEventTypes|String collection|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|signInIdentifier|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|signInIdentifierType|signInIdentifierType|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `userPrincipalName`, `phoneNumber`, `proxyAddress`, `qrCode`, `onPremisesUserPrincipalName`, `unknownFutureValue`.|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|tokenIssuerName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|userAgent|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userDisplayName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userId|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [signIn](../resources/signin.md)|
|userType|signInUserType|**TODO: Add Description** Inherited from [signIn](../resources/signin.md). Possible values are: `member`, `guest`, `unknownFutureValue`.|
|targetTenantId|Guid|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [restrictedSignIn](../resources/restrictedsignin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_restrictedsignin"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/restrictedSignIns/{restrictedSignInId}
Content-Type: application/json
Content-length: 2218

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "flaggedForReview": "Boolean",
  "homeTenantId": "String",
  "isInteractive": "Boolean",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": "Integer",
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "targetTenantId": "Guid"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.restrictedSignIn",
  "id": "96650862-0862-9665-6208-659662086596",
  "alternateSignInName": "String",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "flaggedForReview": "Boolean",
  "homeTenantId": "String",
  "isInteractive": "Boolean",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "processingTimeInMilliseconds": "Integer",
  "riskDetail": "String",
  "riskEventTypes": [
    "String"
  ],
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String",
  "targetTenantId": "Guid"
}
```
