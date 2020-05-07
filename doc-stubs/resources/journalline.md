---
title: "journalLine resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# journalLine resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List account](../api/journalline-list-account.md)|[account](../resources/account.md) collection|Get the accounts from the account navigation property.|
|[Create account](../api/journalline-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[Delete account](../api/journalline-delete-account.md)|None|Delete an [account](../resources/account.md) object.|
|[Update account](../api/journalline-update-account.md)|[account](../resources/account.md)|Update the properties of an account object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read the properties and relationships of an [account](../resources/account.md) object.|
|[List journalLines](../api/company-list-journallines.md)|[journalLine](../resources/journalline.md) collection|Get the journalLines from the journalLines navigation property.|
|[Create journalLines](../api/company-post-journallines.md)|[journalLine](../resources/journalline.md)|Create a new journalLines object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|Guid|**TODO: Add Description**|
|accountNumber|String|**TODO: Add Description**|
|amount|Decimal|**TODO: Add Description**|
|comment|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|documentNumber|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lineNumber|Int32|**TODO: Add Description**|
|postingDate|Date|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
  "lineNumber": "Integer",
  "accountId": "Guid",
  "accountNumber": "String",
  "postingDate": "Date",
  "documentNumber": "String",
  "externalDocumentNumber": "String",
  "amount": "Decimal",
  "description": "String",
  "comment": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```

