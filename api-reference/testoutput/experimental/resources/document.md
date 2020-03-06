---
title: "document resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# document resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get document](../api/document-get.md)|[document](../resources/document.md)|Read properties and relationships of the [document](../resources/document.md) object.|
|[Update document](../api/document-update.md)|[document](../resources/document.md)|Update the properties of a [document](../resources/document.md) object.|
|[List comments](../api/document-list-comments.md)|[documentComment](../resources/documentcomment.md) collection|Get the documentComments from the comments navigation property.|
|[Add comments](../api/document-post-comments.md)|[documentComment](../resources/documentcomment.md)|Add comments by posting to the comments collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|comments|[documentComment](../resources/documentcomment.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.document",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.document",
  "id": "String (identifier)"
}
```

