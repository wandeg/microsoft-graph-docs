---
title: "Update riskDetection"
description: "Update the properties of a riskDetection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update riskDetection

Namespace: microsoft.graph

Update the properties of a [riskDetection](../resources/riskdetection.md) object.

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
PATCH /riskDetections/{riskDetectionsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [riskDetection](../resources/riskdetection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_riskdetection"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/riskDetections/{riskDetectionsId}
Content-Type: application/json
Content-length: 1162

{
  "@odata.type": "#microsoft.graph.riskDetection",
  "requestId": "Request Id value",
  "correlationId": "Correlation Id value",
  "riskEventType": "Risk Event Type value",
  "riskType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "Source value",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "Ip Address value",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
  "detectedDateTime": "2016-12-31T23:59:49.2842106+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
  "userId": "User Id value",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "additionalInfo": "Additional Info value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "b5a8acc2-acc2-b5a8-c2ac-a8b5c2aca8b5",
  "requestId": "Request Id value",
  "correlationId": "Correlation Id value",
  "riskEventType": "Risk Event Type value",
  "riskType": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "source": "Source value",
  "detectionTimingType": "String",
  "activity": "String",
  "tokenIssuerType": "String",
  "ipAddress": "Ip Address value",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation",
    "city": "City value",
    "state": "State value",
    "countryOrRegion": "Country Or Region value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.geoCoordinates",
      "altitude": "Double",
      "latitude": "Double",
      "longitude": "Double"
    }
  },
  "activityDateTime": "2017-01-01T00:03:07.3452024+03:00",
  "detectedDateTime": "2016-12-31T23:59:49.2842106+03:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:57.2159356+03:00",
  "userId": "User Id value",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "additionalInfo": "Additional Info value"
}
```

