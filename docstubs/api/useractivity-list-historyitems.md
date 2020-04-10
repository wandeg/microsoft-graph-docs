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
<!-- {
  "blockType": "request",
  "name": "get_activityhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/activities/{userActivityId}/historyItems
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.activityhistoryitem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 585

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityHistoryItem",
      "id": "a5680261-0261-a568-6102-68a5610268a5",
      "status": "String",
      "activeDurationSeconds": 5,
      "createdDateTime": "2016-12-31T23:58:51.3349474+00:00",
      "lastActiveDateTime": "2016-12-31T23:57:25.6061579+00:00",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
      "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
      "startedDateTime": "2016-12-31T23:59:05.4354214+00:00",
      "userTimezone": "User Timezone value"
    }
  ]
}
```

