---
title: "Add rows"
description: "Add rows by posting to the rows collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add rows

Namespace: microsoft.graph

Add rows by posting to the rows collection.

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
POST ** Collection URI for microsoft.graph.workbookRangeView not found/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookRangeView](../resources/workbookrangeview.md) object.

The following table shows the properties that are required when you create the [workbookRangeView](../resources/workbookrangeview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|cellAddresses|[Json](../resources/json.md)||
|columnCount|Int32||
|formulas|[Json](../resources/json.md)||
|formulasLocal|[Json](../resources/json.md)||
|formulasR1C1|[Json](../resources/json.md)||
|index|Int32||
|numberFormat|[Json](../resources/json.md)||
|rowCount|Int32||
|text|[Json](../resources/json.md)||
|valueTypes|[Json](../resources/json.md)||
|values|[Json](../resources/json.md)||



## Response
If successful, this method returns a `201 Created` response code and a [workbookRangeView](../resources/workbookrangeview.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookrangeview_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeView not found
Content-type: application/json
Content-length: 656

{
  "@odata.type": "#microsoft.graph.workbookRangeView",
  "cellAddresses": {
    "@odata.type": "microsoft.graph.Json"
  },
  "columnCount": 11,
  "formulas": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasLocal": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasR1C1": {
    "@odata.type": "microsoft.graph.Json"
  },
  "index": 5,
  "numberFormat": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rowCount": 8,
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
  "@odata.type": "microsoft.graph.workbookrangeview"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 705

{
  "@odata.type": "#microsoft.graph.workbookRangeView",
  "id": "77bd3e84-3e84-77bd-843e-bd77843ebd77",
  "cellAddresses": {
    "@odata.type": "microsoft.graph.Json"
  },
  "columnCount": 11,
  "formulas": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasLocal": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasR1C1": {
    "@odata.type": "microsoft.graph.Json"
  },
  "index": 5,
  "numberFormat": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rowCount": 8,
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

