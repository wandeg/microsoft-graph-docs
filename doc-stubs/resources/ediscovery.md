---
title: "ediscovery resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ediscovery resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List ediscoveries](../api/ediscovery-list.md)|[ediscovery](../resources/ediscovery.md) collection|Get a list of the [ediscovery](../resources/ediscovery.md) objects and their properties.|
|[Create ediscovery](../api/ediscovery-create.md)|[ediscovery](../resources/ediscovery.md)|Create a new [ediscovery](../resources/ediscovery.md) object.|
|[Get ediscovery](../api/ediscovery-get.md)|[ediscovery](../resources/ediscovery.md)|Read the properties and relationships of an [ediscovery](../resources/ediscovery.md) object.|
|[Update ediscovery](../api/ediscovery-update.md)|[ediscovery](../resources/ediscovery.md)|Update the properties of an [ediscovery](../resources/ediscovery.md) object.|
|[Delete ediscovery](../api/ediscovery-delete.md)|None|Deletes an [ediscovery](../resources/ediscovery.md) object.|
|[List cases](../api/ediscovery-list-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md) collection|Get the ediscoveryCases from the cases navigation property.|
|[Create cases](../api/ediscovery-post-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Create a new cases object.|
|[Get cases](../api/ediscovery-get-ediscoverycase.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Read the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.|
|[Update cases](../api/ediscovery-update-cases.md)|[ediscoveryCase](../resources/ediscoverycase.md)|Update the properties of a cases object.|
|[Delete cases](../api/ediscovery-delete-cases.md)|None|Delete an [ediscoveryCase](../resources/ediscoverycase.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cases|[ediscoveryCase](../resources/ediscoverycase.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery",
  "id": "String (identifier)"
}
```

