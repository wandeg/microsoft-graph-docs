---
title: "item resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# item resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get item](../api/item-get.md)|[item](../resources/item.md)|Read the properties and relationships of an [item](../resources/item.md) object.|
|[Update item](../api/item-update.md)|[item](../resources/item.md)|Update the properties of an [item](../resources/item.md) object.|
|[List picture](../api/item-list-picture.md)|[picture](../resources/picture.md) collection|Get the pictures from the picture navigation property.|
|[Create picture](../api/item-post-picture.md)|[picture](../resources/picture.md)|Create a new picture object.|
|[Delete picture](../api/item-delete-picture.md)|None|Delete a [picture](../resources/picture.md) object.|
|[Update picture](../api/item-update-picture.md)|[picture](../resources/picture.md)|Update the properties of a picture object.|
|[Get picture](../api/picture-get.md)|[picture](../resources/picture.md)|Read the properties and relationships of a [picture](../resources/picture.md) object.|
|[List itemCategory](../api/item-list-itemcategory.md)|[itemCategory](../resources/itemcategory.md) collection|Get the itemCategories from the itemCategory navigation property.|
|[Create itemCategory](../api/item-post-itemcategory.md)|[itemCategory](../resources/itemcategory.md)|Create a new itemCategory object.|
|[Delete itemCategory](../api/item-delete-itemcategory.md)|None|Delete an [itemCategory](../resources/itemcategory.md) object.|
|[Update itemCategory](../api/item-update-itemcategory.md)|[itemCategory](../resources/itemcategory.md)|Update the properties of an itemCategory object.|
|[Get itemCategory](../api/itemcategory-get.md)|[itemCategory](../resources/itemcategory.md)|Read the properties and relationships of an [itemCategory](../resources/itemcategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|baseUnitOfMeasureId|Guid|**TODO: Add Description**|
|blocked|Boolean|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|gtin|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|inventory|Decimal|**TODO: Add Description**|
|itemCategoryCode|String|**TODO: Add Description**|
|itemCategoryId|Guid|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|number|String|**TODO: Add Description**|
|priceIncludesTax|Boolean|**TODO: Add Description**|
|taxGroupCode|String|**TODO: Add Description**|
|taxGroupId|Guid|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|unitCost|Decimal|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|itemCategory|[itemCategory](../resources/itemcategory.md)|**TODO: Add Description**|
|picture|[picture](../resources/picture.md) collection|**TODO: Add Description**|

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

