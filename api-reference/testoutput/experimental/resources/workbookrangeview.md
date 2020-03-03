---
title: "workbookRangeView resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# workbookRangeView resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRangeViews](../api/workbookrangeview-list.md)|[workbookRangeView](../resources/workbookRangeView.md) collection|List properties and relationships of the [workbookRangeView](../resources/workbookrangeview.md) objects.|
|[Get workbookRangeView](../api/workbookrangeview-get.md)|[workbookRangeView](../resources/workbookRangeView.md)|Read properties and relationships of the [workbookRangeView](../resources/workbookrangeview.md) object.|
|[Create workbookRangeView](../api/workbookrangeview-create.md)|[workbookRangeView](../resources/workbookRangeView.md)|Create a new [workbookRangeView](../resources/workbookrangeview.md) object.|
|[Delete workbookRangeView](../api/workbookrangeview-delete.md)|None|Deletes a [workbookRangeView](../resources/workbookrangeview.md).|
|[Update workbookRangeView](../api/workbookrangeview-update.md)|[workbookRangeView](../resources/workbookRangeView.md)|Update the properties of a [workbookRangeView](../resources/workbookrangeview.md) object.|
|[List rows](../api/workbookrangeview-list-rows.md)|[workbookRangeView](../resources/workbookRangeView.md) collection|Get the workbookRangeViews from the rows navigation property.|
|[Add rows](../api/workbookrangeview-post-rows.md)|[workbookRangeView](../resources/workbookRangeView.md)|Add rows by posting to the rows collection.|
|[List rows](../api/workbookrangeview-list-rows.md)|[workbookRangeView](../resources/workbookRangeView.md) collection|Get the workbookRangeViews from the rows navigation property.|
|[Add rows](../api/workbookrangeview-post-rows.md)|[workbookRangeView](../resources/workbookRangeView.md)|Add rows by posting to the rows collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|cellAddresses|[Json](../resources/Json.md)||
|columnCount|Int32||
|formulas|[Json](../resources/Json.md)||
|formulasLocal|[Json](../resources/Json.md)||
|formulasR1C1|[Json](../resources/Json.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|index|Int32||
|numberFormat|[Json](../resources/Json.md)||
|rowCount|Int32||
|text|[Json](../resources/Json.md)||
|values|[Json](../resources/Json.md)||
|valueTypes|[Json](../resources/Json.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|rows|[workbookRangeView](../resources/workbookRangeView.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRangeView",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRangeView",
  "id": "String (identifier)",
  "cellAddresses": {
    "@odata.type": "microsoft.graph.Json"
  },
  "columnCount": 1024,
  "formulas": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasLocal": {
    "@odata.type": "microsoft.graph.Json"
  },
  "formulasR1C1": {
    "@odata.type": "microsoft.graph.Json"
  },
  "index": 1024,
  "numberFormat": {
    "@odata.type": "microsoft.graph.Json"
  },
  "rowCount": 1024,
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

