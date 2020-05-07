---
title: "Create riskDetection"
description: "Create a new riskDetection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create riskDetection

Namespace: microsoft.graph

Create a new [riskDetection](../resources/riskdetection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
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
POST /riskDetections
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [riskDetection](../resources/riskdetection.md) object.

The following table shows the properties that are required when you create the [riskDetection](../resources/riskdetection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|requestId|String|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description**|
|riskEventType|String|**TODO: Add Description**|
|riskType|riskEventType|**TODO: Add Description**. Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description**. Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskLevel|riskLevel|**TODO: Add Description**. Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskDetail|riskDetail|**TODO: Add Description**. Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|source|String|**TODO: Add Description**|
|detectionTimingType|riskDetectionTimingType|**TODO: Add Description**. Possible values are: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|activity|activityType|**TODO: Add Description**. Possible values are: `signin`, `user`, `unknownFutureValue`.|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description**. Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|ipAddress|String|**TODO: Add Description**|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description**|
|activityDateTime|DateTimeOffset|**TODO: Add Description**|
|detectedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|additionalInfo|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [riskDetection](../resources/riskdetection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_riskdetection_from_riskdetections"
}
-->
``` http
POST https://graph.microsoft.com/beta/riskDetections
Content-Type: application/json
Content-length: 721

{
  "@odata.type": "#microsoft.graph.riskDetection",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskdetection"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "3a838ca7-8ca7-3a83-a78c-833aa78c833a",
  "requestId": "String",
  "correlationId": "String",
  "riskEventType": "String",
  "riskType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "String",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "String",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "activityDateTime": "String (timestamp)",
  "detectedDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "userId": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "additionalInfo": "String"
}
```

