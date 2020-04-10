---
title: "dimensionValue resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# dimensionValue resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get dimensionValue](../api/dimensionvalue-get.md)|[dimensionValue](../resources/dimensionvalue.md)|Read properties and relationships of the [dimensionValue](../resources/dimensionvalue.md) object.|
|[Update dimensionValue](../api/dimensionvalue-update.md)|[dimensionValue](../resources/dimensionvalue.md)|Update the properties of a [dimensionValue](../resources/dimensionvalue.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dimensionValue",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dimensionValue",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

