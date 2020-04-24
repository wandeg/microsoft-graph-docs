---
title: "teamsCatalogApp resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamsCatalogApp resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get teamsCatalogApp](../api/teamscatalogapp-get.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Read the properties and relationships of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.|
|[Update teamsCatalogApp](../api/teamscatalogapp-update.md)|[teamsCatalogApp](../resources/teamscatalogapp.md)|Update the properties of a [teamsCatalogApp](../resources/teamscatalogapp.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|distributionMethod|teamsAppDistributionMethod|**TODO: Add Description**. Possible values are: `store`, `organization`, `sideloaded`, `unknownFutureValue`.|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
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

