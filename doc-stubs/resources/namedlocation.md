---
title: "namedLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# namedLocation resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List namedLocations](../api/conditionalaccessroot-list-namedlocations.md)|[namedLocation](../resources/namedlocation.md) collection|Get the namedLocations from the namedLocations navigation property.|
|[Create namedLocations](../api/conditionalaccessroot-post-namedlocations.md)|[namedLocation](../resources/namedlocation.md)|Create a new namedLocations object.|
|[Update namedLocations](../api/conditionalaccessroot-update-namedlocations.md)|[namedLocation](../resources/namedlocation.md)|Update the properties of a namedLocations object.|
|[Get namedLocations](../api/conditionalaccessroot-get-namedlocation.md)|[namedLocation](../resources/namedlocation.md)|Read the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.|
|[Delete namedLocations](../api/conditionalaccessroot-delete-namedlocations.md)|None|Delete a [namedLocation](../resources/namedlocation.md) object.|
|[List namedLocations](../api/namedlocation-list.md)|[namedLocation](../resources/namedlocation.md) collection|Get a list of the [namedLocation](../resources/namedlocation.md) objects and their properties.|
|[Create namedLocation](../api/namedlocation-create.md)|[namedLocation](../resources/namedlocation.md)|Create a new [namedLocation](../resources/namedlocation.md) object.|
|[Get namedLocation](../api/namedlocation-get.md)|[namedLocation](../resources/namedlocation.md)|Read the properties and relationships of a [namedLocation](../resources/namedlocation.md) object.|
|[Update namedLocation](../api/namedlocation-update.md)|[namedLocation](../resources/namedlocation.md)|Update the properties of a [namedLocation](../resources/namedlocation.md) object.|
|[Delete namedLocation](../api/namedlocation-delete.md)|None|Deletes a [namedLocation](../resources/namedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

