---
title: "workbookChartFont resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookChartFont resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookChartFonts](../api/workbookchartfont-list.md)|[workbookChartFont](../resources/workbookchartfont.md) collection|List properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) objects.|
|[Get workbookChartFont](../api/workbookchartfont-get.md)|[workbookChartFont](../resources/workbookchartfont.md)|Read properties and relationships of the [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Create workbookChartFont](../api/workbookchartfont-create.md)|[workbookChartFont](../resources/workbookchartfont.md)|Create a new [workbookChartFont](../resources/workbookchartfont.md) object.|
|[Delete workbookChartFont](../api/workbookchartfont-delete.md)|None|Deletes a [workbookChartFont](../resources/workbookchartfont.md).|
|[Update workbookChartFont](../api/workbookchartfont-update.md)|[workbookChartFont](../resources/workbookchartfont.md)|Update the properties of a [workbookChartFont](../resources/workbookchartfont.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|bold|Boolean||
|color|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|italic|Boolean||
|name|String||
|size|Double||
|underline|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookChartFont",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookChartFont",
  "id": "String (identifier)",
  "bold": true,
  "color": "String",
  "italic": true,
  "name": "String",
  "size": "Double",
  "underline": "String"
}
```

