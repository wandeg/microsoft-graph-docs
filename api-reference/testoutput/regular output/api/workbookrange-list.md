---
title: "List workbookRanges"
description: "List properties and relationships of the workbookRange objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List workbookRanges

Namespace: microsoft.graph

List properties and relationships of the [workbookRange](../resources/workbookrange.md) objects.

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
GET ** Collection URI for microsoft.graph.workbookRange not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [workbookRange](../resources/workbookrange.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookrange"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRange not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.workbookrange)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 978

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.workbookRange",
      "id": "a64cf4a5-f4a5-a64c-a5f4-4ca6a5f44ca6",
      "address": "Address value",
      "addressLocal": "Address Local value",
      "cellCount": 9,
      "columnCount": 11,
      "columnHidden": true,
      "columnIndex": 11,
      "formulas": {
        "@odata.type": "microsoft.graph.Json"
      },
      "formulasLocal": {
        "@odata.type": "microsoft.graph.Json"
      },
      "formulasR1C1": {
        "@odata.type": "microsoft.graph.Json"
      },
      "hidden": true,
      "numberFormat": {
        "@odata.type": "microsoft.graph.Json"
      },
      "rowCount": 8,
      "rowHidden": true,
      "rowIndex": 8,
      "text": {
        "@odata.type": "microsoft.graph.Json"
      },
      "valueTypes": {
        "@odata.type": "microsoft.graph.Json"
      },
      "values": {
        "@odata.type": "microsoft.graph.Json"
      }
    }
  ]
}
```

