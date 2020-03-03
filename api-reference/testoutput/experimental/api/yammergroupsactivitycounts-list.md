---
title: "List yammerGroupsActivityCountses"
description: "List properties and relationships of the yammerGroupsActivityCounts objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List yammerGroupsActivityCountses

Namespace: microsoft.graph

List properties and relationships of the [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) objects.

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
GET ** Collection URI for microsoft.graph.yammerGroupsActivityCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_yammergroupsactivitycounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.yammerGroupsActivityCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.yammergroupsactivitycounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 326

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.yammerGroupsActivityCounts",
      "id": "64d35fa4-5fa4-64d3-a45f-d364a45fd364",
      "reportRefreshDate": "Date",
      "liked": 5,
      "posted": 6,
      "read": 4,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```

