---
title: "workbookRangeFill resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookRangeFill resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List fill](../api/workbookrangeformat-list-fill.md)|[workbookRangeFill](../resources/workbookrangefill.md) collection|Get the workbookRangeFills from the fill navigation property.|
|[Create fill](../api/workbookrangeformat-post-fill.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Create a new fill object.|
|[Delete fill](../api/workbookrangeformat-delete-fill.md)|None|Delete a [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[Update fill](../api/workbookrangeformat-update-fill.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Update the properties of a fill object.|
|[Get fill](../api/workbookrangeformat-get-workbookrangefill.md)|[workbookRangeFill](../resources/workbookrangefill.md)|Read the properties and relationships of a [workbookRangeFill](../resources/workbookrangefill.md) object.|
|[clear](../api/workbookrangefill-clear.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

