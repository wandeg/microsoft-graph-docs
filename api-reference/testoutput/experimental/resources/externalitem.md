---
title: "externalItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# externalItem resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List externalItems](../api/externalitem-list.md)|[externalItem](../resources/externalitem.md) collection|List properties and relationships of the [externalItem](../resources/externalitem.md) objects.|
|[Get externalItem](../api/externalitem-get.md)|[externalItem](../resources/externalitem.md)|Read properties and relationships of the [externalItem](../resources/externalitem.md) object.|
|[Create externalItem](../api/externalitem-create.md)|[externalItem](../resources/externalitem.md)|Create a new [externalItem](../resources/externalitem.md) object.|
|[Delete externalItem](../api/externalitem-delete.md)|None|Deletes a [externalItem](../resources/externalitem.md).|
|[Update externalItem](../api/externalitem-update.md)|[externalItem](../resources/externalitem.md)|Update the properties of a [externalItem](../resources/externalitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acl|[acl](../resources/acl.md) collection||
|content|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|properties|[properties](../resources/properties.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalItem",
  "id": "String (identifier)",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": "String",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl"
    }
  ]
}
```

