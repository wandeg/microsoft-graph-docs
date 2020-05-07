---
title: "paymentTerm resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# paymentTerm resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|calculateDiscountOnCreditMemos|Boolean|**TODO: Add Description**|
|code|String|**TODO: Add Description**|
|discountDateCalculation|String|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|dueDateCalculation|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
  "discountPercent": "Decimal",
  "calculateDiscountOnCreditMemos": "Boolean",
  "lastModifiedDateTime": "String (timestamp)"
}
```

