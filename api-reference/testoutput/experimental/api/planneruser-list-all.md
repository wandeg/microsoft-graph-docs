---
title: "List all"
description: "Get the plannerDeltas from the all navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List all

Get the plannerDeltas from the all navigation property.

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
GET /me/planner/all
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerDelta](../resources/plannerdelta.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerdelta"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/me/planner/all
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannerdelta)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 144

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerDelta",
      "id": "241acbc6-cbc6-241a-c6cb-1a24c6cb1a24"
    }
  ]
}
```

