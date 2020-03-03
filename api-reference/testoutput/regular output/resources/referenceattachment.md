---
title: "referenceAttachment resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# referenceAttachment resource type


Namespace: microsoft.graph




Inherits from [attachment](../resources/attachment.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List referenceAttachments](../api/referenceattachment-list.md)|[referenceAttachment](../resources/referenceattachment.md) collection|List properties and relationships of the [referenceAttachment](../resources/referenceattachment.md) objects.|
|[Get referenceAttachment](../api/referenceattachment-get.md)|[referenceAttachment](../resources/referenceattachment.md)|Read properties and relationships of the [referenceAttachment](../resources/referenceattachment.md) object.|
|[Create referenceAttachment](../api/referenceattachment-create.md)|[referenceAttachment](../resources/referenceattachment.md)|Create a new [referenceAttachment](../resources/referenceattachment.md) object.|
|[Delete referenceAttachment](../api/referenceattachment-delete.md)|None|Deletes a [referenceAttachment](../resources/referenceattachment.md).|
|[Update referenceAttachment](../api/referenceattachment-update.md)|[referenceAttachment](../resources/referenceattachment.md)|Update the properties of a [referenceAttachment](../resources/referenceattachment.md) object.|

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
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.referenceAttachment",
  "baseType": "microsoft.graph.attachment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.referenceAttachment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "contentType": "String",
  "size": 1024,
  "isInline": true
}
```

