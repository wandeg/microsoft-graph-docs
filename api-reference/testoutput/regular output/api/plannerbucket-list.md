---
title: "List plannerBuckets"
description: "List properties and relationships of the plannerBucket objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List plannerBuckets

Namespace: microsoft.graph

List properties and relationships of the [plannerBucket](../resources/plannerbucket.md) objects.

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
GET /planner/buckets
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerbucket"
}
-->
``` http
GET https://graph.microsoft.com/localtest/planner/buckets
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannerbucket)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerBucket",
      "id": "418b73d2-73d2-418b-d273-8b41d2738b41",
      "name": "Name value",
      "planId": "Plan Id value",
      "orderHint": "Order Hint value"
    }
  ]
}
```

