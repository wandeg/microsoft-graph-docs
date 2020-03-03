---
title: "List relyingPartyDetailedSummaries"
description: "List properties and relationships of the relyingPartyDetailedSummary objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List relyingPartyDetailedSummaries

Namespace: microsoft.graph

List properties and relationships of the [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) objects.

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
GET ** Collection URI for microsoft.graph.relyingPartyDetailedSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [relyingPartyDetailedSummary](../resources/relyingpartydetailedsummary.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_relyingpartydetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.relyingPartyDetailedSummary not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.relyingpartydetailedsummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 761

{
  "value": [
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
  ]
}
```

