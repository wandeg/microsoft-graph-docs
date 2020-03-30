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
GET /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}/history
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
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}/history
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyuserhistoryitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 757

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "df8fec0d-ec0d-df8f-0dec-8fdf0dec8fdf",
      "isDeleted": true,
      "isGuest": true,
      "isProcessing": true,
      "riskLastUpdatedDateTime": "2017-01-01T00:02:53.4636668+00:00",
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
        "detail": "String"
      }
    }
  ]
}
```

