---
title: "agedAccountsPayable resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# agedAccountsPayable resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get agedAccountsPayable](../api/agedaccountspayable-get.md)|[agedAccountsPayable](../resources/agedaccountspayable.md)|Read properties and relationships of the [agedAccountsPayable](../resources/agedaccountspayable.md) object.|
|[Update agedAccountsPayable](../api/agedaccountspayable-update.md)|[agedAccountsPayable](../resources/agedaccountspayable.md)|Update the properties of a [agedAccountsPayable](../resources/agedaccountspayable.md) object.|
|[List agedAccountsPayable](../api/company-list-agedaccountspayable.md)|[agedAccountsPayable](../resources/agedaccountspayable.md) collection|Get the agedAccountsPayables from the agedAccountsPayable navigation property.|
|[Add agedAccountsPayable](../api/company-post-agedaccountspayable.md)|[agedAccountsPayable](../resources/agedaccountspayable.md)|Add agedAccountsPayable by posting to the agedAccountsPayable collection.|

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

## JSON representation
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

