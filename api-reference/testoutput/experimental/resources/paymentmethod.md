---
title: "paymentMethod resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# paymentMethod resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List paymentMethods](../api/paymentmethod-list.md)|[paymentMethod](../resources/paymentmethod.md) collection|List properties and relationships of the [paymentMethod](../resources/paymentmethod.md) objects.|
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read properties and relationships of the [paymentMethod](../resources/paymentmethod.md) object.|
|[Create paymentMethod](../api/paymentmethod-create.md)|[paymentMethod](../resources/paymentmethod.md)|Create a new [paymentMethod](../resources/paymentmethod.md) object.|
|[Delete paymentMethod](../api/paymentmethod-delete.md)|None|Deletes a [paymentMethod](../resources/paymentmethod.md).|
|[Update paymentMethod](../api/paymentmethod-update.md)|[paymentMethod](../resources/paymentmethod.md)|Update the properties of a [paymentMethod](../resources/paymentmethod.md) object.|

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
  "@odata.type": "microsoft.graph.paymentMethod",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.paymentMethod",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

