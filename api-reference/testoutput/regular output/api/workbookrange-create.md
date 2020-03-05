---
title: "Create workbookRange"
description: "Create a new workbookRange object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookRange

Namespace: microsoft.graph

Create a new [workbookRange](../resources/workbookrange.md) object.

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
POST ** Collection URI for microsoft.graph.workbookRange not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookRange](../resources/workbookrange.md) object.

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
|formulas|[Json](../resources/json.md)||
|formulasLocal|[Json](../resources/json.md)||
|formulasR1C1|[Json](../resources/json.md)||
|hidden|Boolean||
|numberFormat|[Json](../resources/json.md)||
|rowCount|Int32||
|rowHidden|Boolean||
|rowIndex|Int32||
|text|[Json](../resources/json.md)||
|valueTypes|[Json](../resources/json.md)||
|values|[Json](../resources/json.md)||



## Response
If successful, this method returns a `201 Created` response code and a [workbookRange](../resources/workbookrange.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookrange_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRange not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrange"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 813

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
```

