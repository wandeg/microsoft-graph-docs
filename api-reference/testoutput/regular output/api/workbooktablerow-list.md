---
title: "List workbookTableRows"
description: "List properties and relationships of the workbookTableRow objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookTableRows

Namespace: microsoft.graph

List properties and relationships of the [workbookTableRow](../resources/workbooktablerow.md) objects.

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
GET /me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookTableRow](../resources/workbooktablerow.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbooktablerow"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/drive/items/{driveItemId}/workbook/names/{workbookNamedItemId}/worksheet/tables/{workbookTableId}/rows
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbooktablerow)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookTableRow",
      "id": "a3512edf-2edf-a351-df2e-51a3df2e51a3",
      "index": 5,
      "values": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```

