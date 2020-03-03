---
title: "onenoteResource resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onenoteResource resource type


Namespace: microsoft.graph




Inherits from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List onenoteResources](../api/onenoteresource-list.md)|[onenoteResource](../resources/onenoteresource.md) collection|List properties and relationships of the [onenoteResource](../resources/onenoteresource.md) objects.|
|[Get onenoteResource](../api/onenoteresource-get.md)|[onenoteResource](../resources/onenoteresource.md)|Read properties and relationships of the [onenoteResource](../resources/onenoteresource.md) object.|
|[Create onenoteResource](../api/onenoteresource-create.md)|[onenoteResource](../resources/onenoteresource.md)|Create a new [onenoteResource](../resources/onenoteresource.md) object.|
|[Delete onenoteResource](../api/onenoteresource-delete.md)|None|Deletes a [onenoteResource](../resources/onenoteresource.md).|
|[Update onenoteResource](../api/onenoteresource-update.md)|[onenoteResource](../resources/onenoteresource.md)|Update the properties of a [onenoteResource](../resources/onenoteresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|contentUrl|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|self|String| Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onenoteResource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onenoteResource",
  "id": "String (identifier)",
  "self": "String",
  "content": "Stream",
  "contentUrl": "String"
}
```

