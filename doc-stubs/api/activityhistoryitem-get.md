---
title: "Get activityHistoryItem"
description: "Read the properties and relationships of an activityHistoryItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get activityHistoryItem

Namespace: microsoft.graph

Read the properties and relationships of an [activityHistoryItem](../resources/activityhistoryitem.md) object.

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
GET /me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
GET /users/{usersId}/activities/{userActivityId}/historyItems/{activityHistoryItemId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_activityhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.activityHistoryItem",
    "id": "302776bf-76bf-3027-bf76-2730bf762730",
    "status": "String",
    "activeDurationSeconds": "Integer",
    "createdDateTime": "String (timestamp)",
    "lastActiveDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "expirationDateTime": "String (timestamp)",
    "startedDateTime": "String (timestamp)",
    "userTimezone": "String"
  }
}
```

