---
title: "List workbookRangeFills"
description: "List properties and relationships of the workbookRangeFill objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookRangeFills

Namespace: microsoft.graph

List properties and relationships of the [workbookRangeFill](../resources/workbookrangefill.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookRangeFill not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookRangeFill](../resources/workbookrangefill.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookrangefill"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeFill not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookrangefill)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 180

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookRangeFill",
      "id": "2de1230a-230a-2de1-0a23-e12d0a23e12d",
      "color": "Color value"
    }
  ]
}
```

