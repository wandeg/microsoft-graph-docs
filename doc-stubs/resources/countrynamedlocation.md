---
title: "countryNamedLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# countryNamedLocation resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [namedLocation](../resources/namedlocation.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List countryNamedLocations](../api/countrynamedlocation-list.md)|[countryNamedLocation](../resources/countrynamedlocation.md) collection|Get a list of the [countryNamedLocation](../resources/countrynamedlocation.md) objects and their properties.|
|[Create countryNamedLocation](../api/countrynamedlocation-create.md)|[countryNamedLocation](../resources/countrynamedlocation.md)|Create a new [countryNamedLocation](../resources/countrynamedlocation.md) object.|
|[Get countryNamedLocation](../api/countrynamedlocation-get.md)|[countryNamedLocation](../resources/countrynamedlocation.md)|Read the properties and relationships of a [countryNamedLocation](../resources/countrynamedlocation.md) object.|
|[Update countryNamedLocation](../api/countrynamedlocation-update.md)|[countryNamedLocation](../resources/countrynamedlocation.md)|Update the properties of a [countryNamedLocation](../resources/countrynamedlocation.md) object.|
|[Delete countryNamedLocation](../api/countrynamedlocation-delete.md)|None|Deletes a [countryNamedLocation](../resources/countrynamedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|countriesAndRegions|String collection|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|displayName|String|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|includeUnknownCountriesAndRegions|Boolean|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.countryNamedLocation",
  "baseType": "microsoft.graph.namedLocation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "countriesAndRegions": [
    "String"
  ],
  "includeUnknownCountriesAndRegions": "Boolean"
}
```

