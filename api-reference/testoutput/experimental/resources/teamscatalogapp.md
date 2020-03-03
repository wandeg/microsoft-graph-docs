---
title: "teamsCatalogApp resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# teamsCatalogApp resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsCatalogApp](../api/teamscatalogapp-get.md)|[teamsCatalogApp](../resources/teamsCatalogApp.md)|Read properties and relationships of the [teamsCatalogApp](../resources/teamscatalogapp.md) object.|
|[Delete teamsCatalogApp](../api/teamscatalogapp-delete.md)|None|Deletes a [teamsCatalogApp](../resources/teamscatalogapp.md).|
|[Update teamsCatalogApp](../api/teamscatalogapp-update.md)|[teamsCatalogApp](../resources/teamsCatalogApp.md)|Update the properties of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|distributionMethod|Enumeration|. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|
|externalId|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsCatalogApp",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsCatalogApp",
  "id": "String (identifier)",
  "externalId": "String",
  "name": "String",
  "distributionMethod": "String"
}
```

