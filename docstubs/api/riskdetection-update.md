---
title: "Update riskDetection"
description: "Update the properties of a riskDetection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update riskDetection

Namespace: microsoft.graph

Update the properties of a [riskDetection](../resources/riskdetection.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [riskDetection](../resources/riskdetection.md) object.

The following table shows the properties that are required when you create the [riskDetection](../resources/riskdetection.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|requestId|String||
|correlationId|String||
|riskEventType|String||
|riskType|Enumeration| Possible values are: `unlikelyTravel`, `anonymizedIPAddress`, `maliciousIPAddress`, `unfamiliarFeatures`, `malwareInfectedIPAddress`, `suspiciousIPAddress`, `leakedCredentials`, `investigationsThreatIntelligence`, `generic`, `adminConfirmedUserCompromised`, `mcasImpossibleTravel`, `mcasSuspiciousInboxManipulationRules`, `investigationsThreatIntelligenceSigninLinked`, `maliciousIPAddressValidCredentialsBlockedIP`, `unknownFutureValue`.|
|riskState|Enumeration| Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|riskLevel|Enumeration| Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskDetail|Enumeration| Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|source|String||
|detectionTimingType|Enumeration| Possible values are: `notDefined`, `realtime`, `nearRealtime`, `offline`, `unknownFutureValue`.|
|activity|Enumeration| Possible values are: `signin`, `user`, `unknownFutureValue`.|
|tokenIssuerType|Enumeration| Possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`.|
|ipAddress|String||
|location|[signInLocation](../resources/signinlocation.md)||
|activityDateTime|DateTimeOffset||
|detectedDateTime|DateTimeOffset||
|lastUpdatedDateTime|DateTimeOffset||
|userId|String||
|userDisplayName|String||
|userPrincipalName|String||
|additionalInfo|String||



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
Content-type: application/json
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
  "activityDateTime": "2017-01-01T00:02:32.3183943+00:00",
  "detectedDateTime": "2017-01-01T00:02:45.9116445+00:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00",
  "userId": "User Id value",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "additionalInfo": "Additional Info value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.riskDetection",
  "id": "87273fc9-3fc9-8727-c93f-2787c93f2787",
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
  "activityDateTime": "2017-01-01T00:02:32.3183943+00:00",
  "detectedDateTime": "2017-01-01T00:02:45.9116445+00:00",
  "lastUpdatedDateTime": "2016-12-31T23:58:15.2250773+00:00",
  "userId": "User Id value",
  "userDisplayName": "User Display Name value",
  "userPrincipalName": "User Principal Name value",
  "additionalInfo": "Additional Info value"
}
```

