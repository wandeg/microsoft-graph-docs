---
title: "itemCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# itemCategory resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get itemCategory](../api/itemcategory-get.md)|[itemCategory](../resources/itemCategory.md)|Read properties and relationships of the [itemCategory](../resources/itemcategory.md) object.|
|[Delete itemCategory](../api/itemcategory-delete.md)|None|Deletes a [itemCategory](../resources/itemcategory.md).|
|[Update itemCategory](../api/itemcategory-update.md)|[itemCategory](../resources/itemCategory.md)|Update the properties of a [itemCategory](../resources/itemcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemCategory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemCategory",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

