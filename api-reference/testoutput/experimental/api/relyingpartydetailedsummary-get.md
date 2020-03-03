---
title: "Get relyingPartyDetailedSummary"
description: "Read properties and relationships of the relyingPartyDetailedSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get relyingPartyDetailedSummary

Namespace: microsoft.graph

Read properties and relationships of the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object.

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
GET ** Entity URI for microsoft.graph.relyingPartyDetailedSummary not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.relyingPartyDetailedSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.relyingPartyDetailedSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 705

{
  "value": {
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
}
```

