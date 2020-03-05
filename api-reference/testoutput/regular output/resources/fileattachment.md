---
title: "fileAttachment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# fileAttachment resource type


Namespace: microsoft.graph




Inherits from [attachment](../resources/attachment.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List fileAttachments](../api/fileattachment-list.md)|[fileAttachment](../resources/fileattachment.md) collection|List properties and relationships of the [fileAttachment](../resources/fileattachment.md) objects.|
|[Get fileAttachment](../api/fileattachment-get.md)|[fileAttachment](../resources/fileattachment.md)|Read properties and relationships of the [fileAttachment](../resources/fileattachment.md) object.|
|[Create fileAttachment](../api/fileattachment-create.md)|[fileAttachment](../resources/fileattachment.md)|Create a new [fileAttachment](../resources/fileattachment.md) object.|
|[Delete fileAttachment](../api/fileattachment-delete.md)|None|Deletes a [fileAttachment](../resources/fileattachment.md).|
|[Update fileAttachment](../api/fileattachment-update.md)|[fileAttachment](../resources/fileattachment.md)|Update the properties of a [fileAttachment](../resources/fileattachment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentBytes|Binary||
|contentId|String||
|contentLocation|String||
|contentType|String| Inherited from [attachment](../resources/attachment.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|isInline|Boolean| Inherited from [attachment](../resources/attachment.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [attachment](../resources/attachment.md)|
|name|String| Inherited from [attachment](../resources/attachment.md)|
|size|Int32| Inherited from [attachment](../resources/attachment.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fileAttachment",
  "baseType": "microsoft.graph.attachment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileAttachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": 1024,
  "isInline": true,
  "contentId": "String",
  "contentLocation": "String",
  "contentBytes": "binary"
}
```

