---
title: "printService resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printService resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printService](../api/printservice-get.md)|[printService](../resources/printservice.md)|Read properties and relationships of the [printService](../resources/printservice.md) object.|
|[Update printService](../api/printservice-update.md)|[printService](../resources/printservice.md)|Update the properties of a [printService](../resources/printservice.md) object.|
|[List endpoints](../api/printservice-list-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md) collection|Get the printServiceEndpoints from the endpoints navigation property.|
|[Create endpoints](../api/printservice-post-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Create endpoints by posting to the endpoints collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|endpoints|[printServiceEndpoint](../resources/printserviceendpoint.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printService",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printService",
  "id": "String (identifier)"
}
```

