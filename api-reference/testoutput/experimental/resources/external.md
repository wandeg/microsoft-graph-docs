---
title: "external resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# external resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get external](../api/external-get.md)|[external](../resources/external.md)|Read properties and relationships of the [external](../resources/external.md) object.|
|[Update external](../api/external-update.md)|[external](../resources/external.md)|Update the properties of a [external](../resources/external.md) object.|
|[List connections](../api/external-list-connections.md)|[externalConnection](../resources/externalconnection.md) collection|Get the externalConnections from the connections navigation property.|
|[Add connections](../api/external-post-connections.md)|[externalConnection](../resources/externalconnection.md)|Add connections by posting to the connections collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connections|[externalConnection](../resources/externalconnection.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
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

