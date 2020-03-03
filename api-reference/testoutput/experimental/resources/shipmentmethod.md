---
title: "shipmentMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# shipmentMethod resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List shipmentMethods](../api/shipmentmethod-list.md)|[shipmentMethod](../resources/shipmentmethod.md) collection|List properties and relationships of the [shipmentMethod](../resources/shipmentmethod.md) objects.|
|[Get shipmentMethod](../api/shipmentmethod-get.md)|[shipmentMethod](../resources/shipmentmethod.md)|Read properties and relationships of the [shipmentMethod](../resources/shipmentmethod.md) object.|
|[Create shipmentMethod](../api/shipmentmethod-create.md)|[shipmentMethod](../resources/shipmentmethod.md)|Create a new [shipmentMethod](../resources/shipmentmethod.md) object.|
|[Delete shipmentMethod](../api/shipmentmethod-delete.md)|None|Deletes a [shipmentMethod](../resources/shipmentmethod.md).|
|[Update shipmentMethod](../api/shipmentmethod-update.md)|[shipmentMethod](../resources/shipmentmethod.md)|Update the properties of a [shipmentMethod](../resources/shipmentmethod.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.shipmentMethod",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.shipmentMethod",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

