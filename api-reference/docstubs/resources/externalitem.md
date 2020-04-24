---
title: "externalItem resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# externalItem resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get externalItem](../api/externalitem-get.md)|[externalItem](../resources/externalitem.md)|Read the properties and relationships of an [externalItem](../resources/externalitem.md) object.|
|[Update externalItem](../api/externalitem-update.md)|[externalItem](../resources/externalitem.md)|Update the properties of an [externalItem](../resources/externalitem.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acl|[acl](../resources/acl.md) collection|**TODO: Add Description**|
|content|[externalItemContent](../resources/externalitemcontent.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|properties|[properties](../resources/properties.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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
  "content": {
    "@odata.type": "microsoft.graph.externalItemContent"
  },
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl"
    }
  ]
}
```

