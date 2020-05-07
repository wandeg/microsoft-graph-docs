---
title: "external resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# external resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[Get external](../api/external-get.md)|[external](../resources/external.md)|Read the properties and relationships of an [external](../resources/external.md) object.|
|[Update external](../api/external-update.md)|[external](../resources/external.md)|Update the properties of an [external](../resources/external.md) object.|
|[List connections](../api/external-list-connections.md)|[externalConnection](../resources/externalconnection.md) collection|Get the externalConnections from the connections navigation property.|
|[Create connections](../api/external-post-connections.md)|[externalConnection](../resources/externalconnection.md)|Create a new connections object.|
|[Delete connections](../api/external-delete-connections.md)|None|Delete a [externalConnection](../resources/externalconnection.md) object.|
|[Update connections](../api/external-update-connections.md)|[externalConnection](../resources/externalconnection.md)|Update the properties of a connections object.|
|[Get externalConnection](../api/externalconnection-get.md)|[externalConnection](../resources/externalconnection.md)|Read the properties and relationships of an [externalConnection](../resources/externalconnection.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connections|[externalConnection](../resources/externalconnection.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.external",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.external",
  "id": "String (identifier)"
}
```

