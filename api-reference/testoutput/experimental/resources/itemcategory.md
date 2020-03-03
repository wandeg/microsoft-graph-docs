---
title: "itemCategory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# itemCategory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List itemCategories](../api/itemcategory-list.md)|[itemCategory](../resources/itemcategory.md) collection|List properties and relationships of the [itemCategory](../resources/itemcategory.md) objects.|
|[Get itemCategory](../api/itemcategory-get.md)|[itemCategory](../resources/itemcategory.md)|Read properties and relationships of the [itemCategory](../resources/itemcategory.md) object.|
|[Create itemCategory](../api/itemcategory-create.md)|[itemCategory](../resources/itemcategory.md)|Create a new [itemCategory](../resources/itemcategory.md) object.|
|[Delete itemCategory](../api/itemcategory-delete.md)|None|Deletes a [itemCategory](../resources/itemcategory.md).|
|[Update itemCategory](../api/itemcategory-update.md)|[itemCategory](../resources/itemcategory.md)|Update the properties of a [itemCategory](../resources/itemcategory.md) object.|

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

