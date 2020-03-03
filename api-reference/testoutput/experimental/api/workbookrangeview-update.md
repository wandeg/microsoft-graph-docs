---
title: "Update workbookRangeView"
description: "Update the properties of a workbookRangeView object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookRangeView

Namespace: microsoft.graph

Update the properties of a [workbookRangeView](../resources/workbookrangeview.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookRangeView not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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
If successful, this method returns a `200 OK` response code and an updated [workbookRangeView](../resources/workbookrangeview.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookrangeview"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookRangeView not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 705

{
  "@odata.type": "#microsoft.graph.workbookRangeView",
  "id": "c38b8b5e-8b5e-c38b-5e8b-8bc35e8b8bc3",
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

