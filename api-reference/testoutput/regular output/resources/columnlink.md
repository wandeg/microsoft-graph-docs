---
title: "columnLink resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# columnLink resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List columnLinks](../api/columnlink-list.md)|[columnLink](../resources/columnlink.md) collection|List properties and relationships of the [columnLink](../resources/columnlink.md) objects.|
|[Get columnLink](../api/columnlink-get.md)|[columnLink](../resources/columnlink.md)|Read properties and relationships of the [columnLink](../resources/columnlink.md) object.|
|[Create columnLink](../api/columnlink-create.md)|[columnLink](../resources/columnlink.md)|Create a new [columnLink](../resources/columnlink.md) object.|
|[Delete columnLink](../api/columnlink-delete.md)|None|Deletes a [columnLink](../resources/columnlink.md).|
|[Update columnLink](../api/columnlink-update.md)|[columnLink](../resources/columnlink.md)|Update the properties of a [columnLink](../resources/columnlink.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.columnLink",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.columnLink",
  "id": "String (identifier)",
  "name": "String"
}
```

