---
title: "paymentTerm resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# paymentTerm resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get paymentTerm](../api/paymentterm-get.md)|[paymentTerm](../resources/paymentTerm.md)|Read properties and relationships of the [paymentTerm](../resources/paymentterm.md) object.|
|[Delete paymentTerm](../api/paymentterm-delete.md)|None|Deletes a [paymentTerm](../resources/paymentterm.md).|
|[Update paymentTerm](../api/paymentterm-update.md)|[paymentTerm](../resources/paymentTerm.md)|Update the properties of a [paymentTerm](../resources/paymentterm.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calculateDiscountOnCreditMemos|Boolean||
|code|String||
|discountDateCalculation|String||
|discountPercent|Decimal||
|displayName|String||
|dueDateCalculation|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.paymentTerm",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.paymentTerm",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "dueDateCalculation": "String",
  "discountDateCalculation": "String",
  "discountPercent": "4.2",
  "calculateDiscountOnCreditMemos": true,
  "lastModifiedDateTime": "String (timestamp)"
}
```

