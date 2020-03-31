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
|[Get paymentMethod](../api/paymentmethod-get.md)|[paymentMethod](../resources/paymentmethod.md)|Read properties and relationships of the [paymentMethod](../resources/paymentmethod.md) object.|
|[Update paymentMethod](../api/paymentmethod-update.md)|[paymentMethod](../resources/paymentmethod.md)|Update the properties of a [paymentMethod](../resources/paymentmethod.md) object.|
|[List paymentMethods](../api/company-list-paymentmethods.md)|[paymentMethod](../resources/paymentmethod.md) collection|Get the paymentMethods from the paymentMethods navigation property.|
|[Add paymentMethods](../api/company-post-paymentmethods.md)|[paymentMethod](../resources/paymentmethod.md)|Add paymentMethods by posting to the paymentMethods collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
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

