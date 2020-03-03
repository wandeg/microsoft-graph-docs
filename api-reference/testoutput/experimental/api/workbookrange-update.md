---
title: "Update workbookRange"
description: "Update the properties of a workbookRange object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookRange

Update the properties of a [workbookRange](../resources/workbookrange.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookRange not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookRange](../resources/workbookRange.md) object.

The following table shows the properties that are required when you create the [workbookRange](../resources/workbookrange.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|address|String||
|addressLocal|String||
|cellCount|Int32||
|columnCount|Int32||
|columnHidden|Boolean||
|columnIndex|Int32||
|formulas|[Json](../resources/Json.md)||
|formulasLocal|[Json](../resources/Json.md)||
|formulasR1C1|[Json](../resources/Json.md)||
|hidden|Boolean||
|numberFormat|[Json](../resources/Json.md)||
|rowCount|Int32||
|rowHidden|Boolean||
|rowIndex|Int32||
|text|[Json](../resources/Json.md)||
|valueTypes|[Json](../resources/Json.md)||
|values|[Json](../resources/Json.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookRange](../resources/workbookrange.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookrange"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.workbookRange not found
Content-type: application/json
Content-length: 764

{
  "@odata.type": "#microsoft.graph.workbookRange",
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
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.workbookRange",
  "id": "8b820912-0912-8b82-1209-828b1209828b",
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
```

