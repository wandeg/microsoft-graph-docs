---
title: "itemAttachment resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# itemAttachment resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [attachment](../resources/attachment.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List item](../api/itemattachment-list-item.md)|[outlookItem](../resources/outlookitem.md) collection|Get the outlookItems from the item navigation property.|
|[Create item](../api/itemattachment-post-item.md)|[outlookItem](../resources/outlookitem.md)|Create a new item object.|
|[Delete item](../api/itemattachment-delete-item.md)|None|Delete an [outlookItem](../resources/outlookitem.md) object.|
|[Update item](../api/itemattachment-update-item.md)|[outlookItem](../resources/outlookitem.md)|Update the properties of an item object.|
|[Get item](../api/itemattachment-get-outlookitem.md)|[outlookItem](../resources/outlookitem.md)|Read the properties and relationships of an [outlookItem](../resources/outlookitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentType|String|**TODO: Add Description** Inherited from [attachment](../resources/attachment.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isInline|Boolean|**TODO: Add Description** Inherited from [attachment](../resources/attachment.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [attachment](../resources/attachment.md)|
|name|String|**TODO: Add Description** Inherited from [attachment](../resources/attachment.md)|
|size|Int32|**TODO: Add Description** Inherited from [attachment](../resources/attachment.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|item|[outlookItem](../resources/outlookitem.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.itemAttachment",
  "baseType": "microsoft.graph.attachment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.itemAttachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": "Integer",
  "isInline": "Boolean"
}
```

