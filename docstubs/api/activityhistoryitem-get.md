---
title: "Get activityHistoryItem"
description: "Read properties and relationships of the activityHistoryItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get activityHistoryItem

Namespace: microsoft.graph

Read properties and relationships of the [activityHistoryItem](../resources/activityhistoryitem.md) object.

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
GET /me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
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
If successful, this method returns a `200 OK` response code and [activityHistoryItem](../resources/activityhistoryitem.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_activityhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/activities/{userActivityId}/historyItems/{activityHistoryItemId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 550

{
  "value": {
    "@odata.type": "#microsoft.graph.activityHistoryItem",
    "id": "eadac954-c954-eada-54c9-daea54c9daea",
    "status": "String",
    "activeDurationSeconds": 5,
    "createdDateTime": "2016-12-31T23:58:10.4520456+03:00",
    "lastActiveDateTime": "2016-12-31T23:58:47.8943563+03:00",
    "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
    "expirationDateTime": "2016-12-31T23:56:49.0349895+03:00",
    "startedDateTime": "2016-12-31T23:57:05.2444922+03:00",
    "userTimezone": "User Timezone value"
  }
}
```

