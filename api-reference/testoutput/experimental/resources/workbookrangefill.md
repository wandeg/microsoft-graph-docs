---
title: "workbookRangeFill resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# workbookRangeFill resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List workbookRangeFills](../api/workbookrangefill-list.md)|[workbookRangeFill](../resources/workbookrangefill.md) collection|List properties and relationships of the [workbookRangeFill](../resources/workbookrangefill.md) objects.|
|[Get workbookRangeFill](../api/workbookrangefill-get.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Read properties and relationships of the [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[Create workbookRangeFill](../api/workbookrangefill-create.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Create a new [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[Delete workbookRangeFill](../api/workbookrangefill-delete.md)|None|Deletes a [workbookRangeFill](../resources/workbookrangefill.md).|
|[Update workbookRangeFill](../api/workbookrangefill-update.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Update the properties of a [workbookRangeFill](../resources/workbookrangefill.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String||
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRangeFill",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRangeFill",
  "id": "String (identifier)",
  "color": "String"
}
```

