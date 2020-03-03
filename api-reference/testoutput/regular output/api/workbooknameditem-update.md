---
title: "Update workbookNamedItem"
description: "Update the properties of a workbookNamedItem object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookNamedItem

Update the properties of a [workbookNamedItem](../resources/workbooknameditem.md) object.

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
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}
PATCH /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/names/{workbookNamedItemId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookNamedItem](../resources/workbookNamedItem.md) object.

The following table shows the properties that are required when you create the [workbookNamedItem](../resources/workbooknameditem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|comment|String||
|name|String||
|scope|String||
|type|String||
|value|[Json](../resources/Json.md)||
|visible|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookNamedItem](../resources/workbooknameditem.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbooknameditem"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.workbookNamedItem",
  "comment": "Comment value",
  "name": "Name value",
  "scope": "Scope value",
  "type": "Type value",
  "value": {
    "@odata.type": "microsoft.graph.Json"
  },
  "visible": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

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
```

