---
title: "List sharePointActivityUserCountses"
description: "List properties and relationships of the sharePointActivityUserCounts objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List sharePointActivityUserCountses

Namespace: microsoft.graph

List properties and relationships of the [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) objects.

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
GET ** Collection URI for microsoft.graph.sharePointActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sharepointactivityusercounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.sharePointActivityUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sharepointactivityusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 406

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharePointActivityUserCounts",
      "id": "b9f3b69c-b69c-b9f3-9cb6-f3b99cb6f3b9",
      "reportRefreshDate": "Date",
      "visitedPage": 11,
      "viewedOrEdited": 14,
      "synced": 6,
      "sharedInternally": 0,
      "sharedExternally": 0,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

