---
title: "itemAttachment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# itemAttachment resource type




Inherits from [attachment](../resources/attachment.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List itemAttachments](../api/itemattachment-list.md)|[itemAttachment](../resources/itemAttachment.md) collection|List properties and relationships of the [itemAttachment](../resources/itemattachment.md) objects.|
|[Get itemAttachment](../api/itemattachment-get.md)|[itemAttachment](../resources/itemAttachment.md)|Read properties and relationships of the [itemAttachment](../resources/itemattachment.md) object.|
|[Create itemAttachment](../api/itemattachment-create.md)|[itemAttachment](../resources/itemAttachment.md)|Create a new [itemAttachment](../resources/itemattachment.md) object.|
|[Delete itemAttachment](../api/itemattachment-delete.md)|None|Deletes a [itemAttachment](../resources/itemattachment.md).|
|[Update itemAttachment](../api/itemattachment-update.md)|[itemAttachment](../resources/itemAttachment.md)|Update the properties of a [itemAttachment](../resources/itemattachment.md) object.|
|[Get outlookItem](../api/outlookitem-get.md)|[outlookItem](../resources/outlookItem.md)|Read properties and relationships of the [outlookItem](../resources/outlookitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentType|String| Inherited from [attachment](../resources/attachment.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isInline|Boolean| Inherited from [attachment](../resources/attachment.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [attachment](../resources/attachment.md)|
|name|String| Inherited from [attachment](../resources/attachment.md)|
|size|Int32| Inherited from [attachment](../resources/attachment.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|item|[outlookItem](../resources/outlookItem.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
  "size": 1024,
  "isInline": true
}
```

