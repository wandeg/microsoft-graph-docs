---
title: "agedAccountsPayable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# agedAccountsPayable resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agedAccountsPayable](../api/agedaccountspayable-get.md)|[agedAccountsPayable](../resources/agedAccountsPayable.md)|Read properties and relationships of the [agedAccountsPayable](../resources/agedaccountspayable.md) object.|
|[Delete agedAccountsPayable](../api/agedaccountspayable-delete.md)|None|Deletes a [agedAccountsPayable](../resources/agedaccountspayable.md).|
|[Update agedAccountsPayable](../api/agedaccountspayable-update.md)|[agedAccountsPayable](../resources/agedAccountsPayable.md)|Update the properties of a [agedAccountsPayable](../resources/agedaccountspayable.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|agedAsOfDate|Date||
|balanceDue|Decimal||
|currencyCode|String||
|currentAmount|Decimal||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|period1Amount|Decimal||
|period2Amount|Decimal||
|period3Amount|Decimal||
|periodLengthFilter|String||
|vendorNumber|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.agedAccountsPayable",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.agedAccountsPayable",
  "id": "String (identifier)",
  "vendorNumber": "String",
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

