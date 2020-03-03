---
title: "Update relyingPartyDetailedSummary"
description: "Update the properties of a relyingPartyDetailedSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update relyingPartyDetailedSummary

Namespace: microsoft.graph

Update the properties of a [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.relyingPartyDetailedSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

The following table shows the properties that are required when you create the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|relyingPartyId|String||
|serviceId|String||
|relyingPartyName|String||
|successfulSignInCount|Int64||
|failedSignInCount|Int64||
|totalSignInCount|Int64||
|signInSuccessRate|Double||
|uniqueUserCount|Int64||
|migrationStatus|Enumeration|. Possible values are: `ready`, `needsReview`, `additionalStepsRequired`, `unknownFutureValue`.|
|migrationValidationDetails|[keyValuePair](../resources/keyvaluepair.md) collection||
|replyUrls|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_relyingpartydetailedsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.relyingPartyDetailedSummary not found
Content-type: application/json
Content-length: 595

{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "relyingPartyId": "Relying Party Id value",
  "serviceId": "Service Id value",
  "relyingPartyName": "Relying Party Name value",
  "successfulSignInCount": 5,
  "failedSignInCount": 1,
  "totalSignInCount": 0,
  "signInSuccessRate": "Double",
  "uniqueUserCount": 15,
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "replyUrls": [
    "Reply Urls value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 644

{
  "@odata.type": "#microsoft.graph.relyingPartyDetailedSummary",
  "id": "463e740e-740e-463e-0e74-3e460e743e46",
  "relyingPartyId": "Relying Party Id value",
  "serviceId": "Service Id value",
  "relyingPartyName": "Relying Party Name value",
  "successfulSignInCount": 5,
  "failedSignInCount": 1,
  "totalSignInCount": 0,
  "signInSuccessRate": "Double",
  "uniqueUserCount": 15,
  "migrationStatus": "String",
  "migrationValidationDetails": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "replyUrls": [
    "Reply Urls value"
  ]
}
```

