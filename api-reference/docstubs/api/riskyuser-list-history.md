---
title: "List history"
description: "Get the riskyUserHistoryItems from the history navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List history

Namespace: microsoft.graph

Get the riskyUserHistoryItems from the history navigation property.

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
GET /riskyUsers/{riskyUsersId}/history
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyuserhistoryitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "1a608df0-8df0-1a60-f08d-601af08d601a",
      "isDeleted": true,
      "isGuest": true,
      "isProcessing": true,
      "riskLastUpdatedDateTime": "2016-12-31T23:58:33.1152347+03:00",
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

