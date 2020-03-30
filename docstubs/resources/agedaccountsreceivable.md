---
title: "agedAccountsReceivable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# agedAccountsReceivable resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agedAccountsReceivable](../api/agedaccountsreceivable-get.md)|[agedAccountsReceivable](../resources/agedaccountsreceivable.md)|Read properties and relationships of the [agedAccountsReceivable](../resources/agedaccountsreceivable.md) object.|
|[Update agedAccountsReceivable](../api/agedaccountsreceivable-update.md)|[agedAccountsReceivable](../resources/agedaccountsreceivable.md)|Update the properties of a [agedAccountsReceivable](../resources/agedaccountsreceivable.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|agedAsOfDate|Date||
|balanceDue|Decimal||
|currencyCode|String||
|currentAmount|Decimal||
|customerNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|period1Amount|Decimal||
|period2Amount|Decimal||
|period3Amount|Decimal||
|periodLengthFilter|String||

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

