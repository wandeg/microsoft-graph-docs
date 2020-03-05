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

## HTTP request
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

## Examples

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
Content-Length: 582

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityHistoryItem",
      "id": "bd768387-8387-bd76-8783-76bd878376bd",
      "status": "String",
      "activeDurationSeconds": 5,
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "lastActiveDateTime": "2016-12-31T23:57:55.9017756+03:00",
      "lastModifiedDateTime": "2017-01-01T00:02:21.89044+03:00",
      "expirationDateTime": "2016-12-31T23:59:11.273206+03:00",
      "startedDateTime": "2017-01-01T00:00:00.0290262+03:00",
      "userTimezone": "User Timezone value"
    }
  ]
}
```

