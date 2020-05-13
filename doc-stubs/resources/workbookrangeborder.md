---
title: "workbookRangeBorder resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookRangeBorder resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List borders](../api/workbookrangeformat-list-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md) collection|Get the workbookRangeBorders from the borders navigation property.|
|[Create borders](../api/workbookrangeformat-post-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Create a new borders object.|
|[Delete borders](../api/workbookrangeformat-delete-borders.md)|None|Delete a [workbookRangeBorder](../resources/workbookrangeborder.md) object.|
|[Update borders](../api/workbookrangeformat-update-borders.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Update the properties of a borders object.|
|[Get borders](../api/workbookrangeformat-get-workbookrangeborder.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|Read the properties and relationships of a [workbookRangeBorder](../resources/workbookrangeborder.md) object.|
|[itemAt](../api/workbookrangeborder-itemat.md)|[workbookRangeBorder](../resources/workbookrangeborder.md)|**TODO: Add Description**|
|[count](../api/workbookrangeborder-count.md)|Int32|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|sideIndex|String|**TODO: Add Description**|
|style|String|**TODO: Add Description**|
|weight|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.workbookRangeBorder",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookRangeBorder",
  "id": "String (identifier)",
  "color": "String",
  "sideIndex": "String",
  "style": "String",
  "weight": "String"
}
```

