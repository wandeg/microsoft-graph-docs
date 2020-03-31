---
title: "journalLine resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# journalLine resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get journalLine](../api/journalline-get.md)|[journalLine](../resources/journalline.md)|Read properties and relationships of the [journalLine](../resources/journalline.md) object.|
|[Update journalLine](../api/journalline-update.md)|[journalLine](../resources/journalline.md)|Update the properties of a [journalLine](../resources/journalline.md) object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|Guid||
|accountNumber|String||
|amount|Decimal||
|comment|String||
|description|String||
|documentNumber|String||
|externalDocumentNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String||
|lastModifiedDateTime|DateTimeOffset||
|lineNumber|Int32||
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
  "@odata.type": "microsoft.graph.journalLine",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.journalLine",
  "id": "String (identifier)",
  "journalDisplayName": "String",
  "lineNumber": 1024,
  "accountId": "Guid",
  "accountNumber": "String",
  "postingDate": "Date",
  "documentNumber": "String",
  "externalDocumentNumber": "String",
  "amount": "4.2",
  "description": "String",
  "comment": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

