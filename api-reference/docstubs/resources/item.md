---
title: "item resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# item resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read properties and relationships of the [item](../resources/item.md) object.|
|[Update item](../api/item-update.md)|[item](../resources/item.md)|Update the properties of a [item](../resources/item.md) object.|
|[List picture](../api/item-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Add picture](../api/item-post-picture.md)|[picture](../resources/picture.md)|Add picture by posting to the picture collection.|
|[Get itemCategory](../api/itemcategory-get.md)|[itemCategory](../resources/itemcategory.md)|Read properties and relationships of the [itemCategory](../resources/itemcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|baseUnitOfMeasureId|Guid||
|blocked|Boolean||
|displayName|String||
|gtin|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|inventory|Decimal||
|itemCategoryCode|String||
|itemCategoryId|Guid||
|lastModifiedDateTime|DateTimeOffset||
|number|String||
|priceIncludesTax|Boolean||
|taxGroupCode|String||
|taxGroupId|Guid||
|type|String||
|unitCost|Decimal||
|unitPrice|Decimal||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|itemCategory|[itemCategory](../resources/itemcategory.md)||
|picture|[picture](../resources/picture.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.item",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.item",
  "id": "String (identifier)",
  "number": "String",
  "displayName": "String",
  "type": "String",
  "itemCategoryId": "Guid",
  "itemCategoryCode": "String",
  "blocked": true,
  "baseUnitOfMeasureId": "Guid",
  "gtin": "String",
  "inventory": "4.2",
  "unitPrice": "4.2",
  "priceIncludesTax": true,
  "unitCost": "4.2",
  "taxGroupId": "Guid",
  "taxGroupCode": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

