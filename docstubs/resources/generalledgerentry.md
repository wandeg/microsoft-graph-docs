---
title: "generalLedgerEntry resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# generalLedgerEntry resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get generalLedgerEntry](../api/generalledgerentry-get.md)|[generalLedgerEntry](../resources/generalledgerentry.md)|Read properties and relationships of the [generalLedgerEntry](../resources/generalledgerentry.md) object.|
|[Update generalLedgerEntry](../api/generalledgerentry-update.md)|[generalLedgerEntry](../resources/generalledgerentry.md)|Update the properties of a [generalLedgerEntry](../resources/generalledgerentry.md) object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|
|[List generalLedgerEntries](../api/company-list-generalledgerentries.md)|[generalLedgerEntry](../resources/generalledgerentry.md) collection|Get the generalLedgerEntries from the generalLedgerEntries navigation property.|
|[Add generalLedgerEntries](../api/company-post-generalledgerentries.md)|[generalLedgerEntry](../resources/generalledgerentry.md)|Add generalLedgerEntries by posting to the generalLedgerEntries collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|Guid||
|accountNumber|String||
|creditAmount|Decimal||
|debitAmount|Decimal||
|description|String||
|documentNumber|String||
|documentType|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||
|postingDate|Date||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.generalLedgerEntry",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.generalLedgerEntry",
  "id": "String (identifier)",
  "postingDate": "Date",
  "documentNumber": "String",
  "documentType": "String",
  "accountId": "Guid",
  "accountNumber": "String",
  "description": "String",
  "debitAmount": "4.2",
  "creditAmount": "4.2",
  "lastModifiedDateTime": "String (timestamp)"
}
```

