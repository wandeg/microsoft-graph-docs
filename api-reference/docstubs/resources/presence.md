---
title: "presence resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# presence resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get presence](../api/presence-get.md)|[presence](../resources/presence.md)|Read the properties and relationships of a [presence](../resources/presence.md) object.|
|[Update presence](../api/presence-update.md)|[presence](../resources/presence.md)|Update the properties of a [presence](../resources/presence.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activity|String|**TODO: Add Description**|
|availability|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.presence",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.presence",
  "id": "String (identifier)",
  "availability": "String",
  "activity": "String"
}
```

