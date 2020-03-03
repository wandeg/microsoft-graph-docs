---
title: "List workbookTableColumns"
description: "List properties and relationships of the workbookTableColumn objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookTableColumns

Namespace: microsoft.graph

List properties and relationships of the [workbookTableColumn](../resources/workbooktablecolumn.md) objects.

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
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookTableColumn](../resources/workbooktablecolumn.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbooktablecolumn"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/columns
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbooktablecolumn)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookTableColumn",
      "id": "e0a80ff4-0ff4-e0a8-f40f-a8e0f40fa8e0",
      "index": 5,
      "name": "Name value",
      "values": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```

