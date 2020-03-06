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
|[Get itemCategory](../api/itemcategory-get.md)|[itemCategory](../resources/itemcategory.md)|Read properties and relationships of the [itemCategory](../resources/itemcategory.md) object.|
|[Update itemCategory](../api/itemcategory-update.md)|[itemCategory](../resources/itemcategory.md)|Update the properties of a [itemCategory](../resources/itemcategory.md) object.|
|[List itemCategories](../api/company-list-itemcategories.md)|[itemCategory](../resources/itemcategory.md) collection|Get the itemCategories from the itemCategories navigation property.|
|[Add itemCategories](../api/company-post-itemcategories.md)|[itemCategory](../resources/itemcategory.md)|Add itemCategories by posting to the itemCategories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
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

