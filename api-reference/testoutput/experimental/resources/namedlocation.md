---
title: "namedLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# namedLocation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get namedLocation](../api/namedlocation-get.md)|[namedLocation](../resources/namedlocation.md)|Read properties and relationships of the [namedLocation](../resources/namedlocation.md) object.|
|[Update namedLocation](../api/namedlocation-update.md)|[namedLocation](../resources/namedlocation.md)|Update the properties of a [namedLocation](../resources/namedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.namedLocation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.namedLocation",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)"
}
```

