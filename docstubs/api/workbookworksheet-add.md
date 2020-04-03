---
title: "add"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# add

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
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/worksheets/add
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



## Response
If successful, this action returns a `200 OK` response code and a [workbookWorksheet](../resources/workbookworksheet.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbookworksheet_add"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/worksheets/add

Content-type: application/json
Content-length: 28

{
  "name": "Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookworksheet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookWorksheet",
    "id": "871cb9b8-b9b8-871c-b8b9-1c87b8b91c87",
    "name": "Name value",
    "position": 8,
    "visibility": "Visibility value"
  }
}
```

