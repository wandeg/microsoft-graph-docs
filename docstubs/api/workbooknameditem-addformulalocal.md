---
title: "addFormulaLocal"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# addFormulaLocal

Namespace: microsoft.graph



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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/addFormulaLocal
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/names/addFormulaLocal
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|name|String||
|formula|String||
|comment|String||



## Response
If successful, this action returns a `200 OK` response code and a [workbookNamedItem](../resources/workbooknameditem.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbooknameditem_addformulalocal"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/addFormulaLocal

Content-type: application/json
Content-length: 90

{
  "name": "Name value",
  "formula": "Formula value",
  "comment": "Comment value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbooknameditem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 338

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookNamedItem",
    "id": "2d439e23-9e23-2d43-239e-432d239e432d",
    "comment": "Comment value",
    "name": "Name value",
    "scope": "Scope value",
    "type": "Type value",
    "value": {
      "@odata.type": "microsoft.graph.Json"
    },
    "visible": true
  }
}
```

