---
title: "List activityHistoryItems"
description: "List properties and relationships of the activityHistoryItem objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List activityHistoryItems

Namespace: microsoft.graph

List properties and relationships of the [activityHistoryItem](../resources/activityhistoryitem.md) objects.

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
GET /me/activities/{userActivityId}/historyItems
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [activityHistoryItem](../resources/activityhistoryitem.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_activityhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/activities/{userActivityId}/historyItems
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.activityhistoryitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 584

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityHistoryItem",
      "id": "c87f6d68-6d68-c87f-686d-7fc8686d7fc8",
      "status": "String",
      "activeDurationSeconds": 5,
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
      "lastActiveDateTime": "2017-01-01T00:01:03.4547516+03:00",
      "lastModifiedDateTime": "2017-01-01T00:00:08.5199759+03:00",
      "expirationDateTime": "2016-12-31T23:58:41.2128216+03:00",
      "startedDateTime": "2017-01-01T00:02:08.4353012+03:00",
      "userTimezone": "User Timezone value"
    }
  ]
}
```

