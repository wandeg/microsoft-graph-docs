---
title: "namedLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# namedLocation resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List namedLocations](../api/namedlocation-list.md)|[namedLocation](../resources/namedLocation.md) collection|List properties and relationships of the [namedLocation](../resources/namedlocation.md) objects.|
|[Get namedLocation](../api/namedlocation-get.md)|[namedLocation](../resources/namedLocation.md)|Read properties and relationships of the [namedLocation](../resources/namedlocation.md) object.|
|[Create namedLocation](../api/namedlocation-create.md)|[namedLocation](../resources/namedLocation.md)|Create a new [namedLocation](../resources/namedlocation.md) object.|
|[Delete namedLocation](../api/namedlocation-delete.md)|None|Deletes a [namedLocation](../resources/namedlocation.md).|
|[Update namedLocation](../api/namedlocation-update.md)|[namedLocation](../resources/namedLocation.md)|Update the properties of a [namedLocation](../resources/namedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
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

