---
title: "List workbookRangeFonts"
description: "List properties and relationships of the workbookRangeFont objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookRangeFonts

List properties and relationships of the [workbookRangeFont](../resources/workbookrangefont.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookRangeFont not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookRangeFont](../resources/workbookrangefont.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookrangefont"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.workbookRangeFont not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookrangefont)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookRangeFont",
      "id": "5d4c5da8-5da8-5d4c-a85d-4c5da85d4c5d",
      "bold": true,
      "color": "Color value",
      "italic": true,
      "name": "Name value",
      "size": "Double",
      "underline": "Underline value"
    }
  ]
}
```

