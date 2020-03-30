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

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
GET https://graph.microsoft.com/beta/me/activities/{userActivityId}/historyItems
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
Content-Length: 583

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityHistoryItem",
      "id": "19f975c1-75c1-19f9-c175-f919c175f919",
      "status": "String",
      "activeDurationSeconds": 5,
      "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
      "lastActiveDateTime": "2016-12-31T23:57:11.703294+00:00",
      "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00",
      "expirationDateTime": "2016-12-31T23:59:40.5485728+00:00",
      "startedDateTime": "2017-01-01T00:03:28.669872+00:00",
      "userTimezone": "User Timezone value"
    }
  ]
}
```

