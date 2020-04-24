---
title: "agedAccountsReceivable resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# agedAccountsReceivable resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agedAccountsReceivable](../api/agedaccountsreceivable-get.md)|[agedAccountsReceivable](../resources/agedaccountsreceivable.md)|Read the properties and relationships of an [agedAccountsReceivable](../resources/agedaccountsreceivable.md) object.|
|[Update agedAccountsReceivable](../api/agedaccountsreceivable-update.md)|[agedAccountsReceivable](../resources/agedaccountsreceivable.md)|Update the properties of an [agedAccountsReceivable](../resources/agedaccountsreceivable.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|agedAsOfDate|Date|**TODO: Add Description**|
|balanceDue|Decimal|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currentAmount|Decimal|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|period1Amount|Decimal|**TODO: Add Description**|
|period2Amount|Decimal|**TODO: Add Description**|
|period3Amount|Decimal|**TODO: Add Description**|
|periodLengthFilter|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agedAccountsReceivable",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agedAccountsReceivable",
  "id": "String (identifier)",
  "customerNumber": "String",
  "name": "String",
  "currencyCode": "String",
  "balanceDue": "4.2",
  "currentAmount": "4.2",
  "period1Amount": "4.2",
  "period2Amount": "4.2",
  "period3Amount": "4.2",
  "agedAsOfDate": "Date",
  "periodLengthFilter": "String"
}
```

