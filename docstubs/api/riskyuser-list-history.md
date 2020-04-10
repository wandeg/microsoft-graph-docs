---
title: "List history"
description: "Get the riskyUserHistoryItems from the history navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List history

Namespace: microsoft.graph

Get the riskyUserHistoryItems from the history navigation property.

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
GET /riskyUsers/{riskyUsersId}/history
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}/history
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyuserhistoryitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 834

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "50a9e6a7-e6a7-50a9-a7e6-a950a7e6a950",
      "isDeleted": true,
      "isGuest": true,
      "isProcessing": true,
      "riskLastUpdatedDateTime": "2016-12-31T23:59:26.9429943+00:00",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "userId": "User Id value",
      "initiatedBy": "Initiated By value",
      "activity": {
        "@odata.type": "microsoft.graph.riskUserActivity",
        "eventTypes": [
          "String"
        ],
        "riskEventTypes": [
          "Risk Event Types value"
        ],
        "detail": "String"
      }
    }
  ]
}
```

