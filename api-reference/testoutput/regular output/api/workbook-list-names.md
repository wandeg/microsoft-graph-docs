---
title: "List names"
description: "Get the workbookNamedItems from the names navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List names

Get the workbookNamedItems from the names navigation property.

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
GET /me/drive/items/{driveItemId}/workbook/names
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookNamedItem](../resources/workbooknameditem.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbooknameditem"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/me/drive/items/{driveItemId}/workbook/names
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbooknameditem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 372

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookNamedItem",
      "id": "2c1a1480-1480-2c1a-8014-1a2c80141a2c",
      "comment": "Comment value",
      "name": "Name value",
      "scope": "Scope value",
      "type": "Type value",
      "value": {
        "@odata.type": "microsoft.graph.Json"
      },
      "visible": true
    }
  ]
}
```

