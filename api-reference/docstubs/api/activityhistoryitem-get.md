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
GET /invitations/{invitationsId}/invitedUser/activities/{userActivityId}/historyItems/{activityHistoryItemId}
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
If successful, this method returns a `200 OK` response code and an [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_activityhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/activities/{userActivityId}/historyItems/{activityHistoryItemId}
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
    "id": "2cffeada-eada-2cff-daea-ff2cdaeaff2c",
    "status": "String",
    "activeDurationSeconds": 5,
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "lastActiveDateTime": "2017-01-01T00:02:01.5517519+03:00",
    "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
    "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
    "startedDateTime": "2017-01-01T00:03:12.189456+03:00",
    "userTimezone": "User Timezone value"
  }
}
```

