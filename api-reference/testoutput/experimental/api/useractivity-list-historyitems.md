---
title: "List historyItems"
description: "Get the activityHistoryItems from the historyItems navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List historyItems

Namespace: microsoft.graph

Get the activityHistoryItems from the historyItems navigation property.

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
      "id": "8f247e5d-7e5d-8f24-5d7e-248f5d7e248f",
      "status": "String",
      "activeDurationSeconds": 5,
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "lastActiveDateTime": "2016-12-31T23:58:54.0663658+03:00",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
      "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
      "startedDateTime": "2016-12-31T23:57:57.4958527+03:00",
      "userTimezone": "User Timezone value"
    }
  ]
}
```

