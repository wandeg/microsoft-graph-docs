---
title: "List itemAnalyticses"
description: "List properties and relationships of the itemAnalytics objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List itemAnalyticses

List properties and relationships of the [itemAnalytics](../resources/itemanalytics.md) objects.

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
GET ** Collection URI for microsoft.graph.itemAnalytics not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [itemAnalytics](../resources/itemanalytics.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemanalytics"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.itemAnalytics not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.itemanalytics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 145

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.itemAnalytics",
      "id": "9d2513b6-13b6-9d25-b613-259db613259d"
    }
  ]
}
```

