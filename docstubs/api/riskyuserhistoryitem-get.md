---
title: "Get riskyUserHistoryItem"
description: "Read properties and relationships of the riskyUserHistoryItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get riskyUserHistoryItem

Namespace: microsoft.graph

Read properties and relationships of the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

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
GET /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
GET /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}/history/{riskyUserHistoryItemId}
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
If successful, this method returns a `200 OK` response code and [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 703

{
  "value": {
    "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
    "id": "dbaf6b49-6b49-dbaf-496b-afdb496bafdb",
    "isDeleted": true,
    "isGuest": true,
    "isProcessing": true,
    "riskLastUpdatedDateTime": "2016-12-31T23:56:36.5905801+03:00",
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
}
```

