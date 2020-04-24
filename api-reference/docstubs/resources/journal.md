---
title: "journal resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# journal resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get journal](../api/journal-get.md)|[journal](../resources/journal.md)|Read the properties and relationships of a [journal](../resources/journal.md) object.|
|[Update journal](../api/journal-update.md)|[journal](../resources/journal.md)|Update the properties of a [journal](../resources/journal.md) object.|
|[post](../api/journal-post.md)|None|**TODO: Add Description**|
|[List account](../api/journal-list-account.md)|[account](../resources/account.md) collection|Get the accounts from the account navigation property.|
|[Create account](../api/journal-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[Delete account](../api/journal-delete-account.md)|None|Delete an [account](../resources/account.md) object.|
|[Update account](../api/journal-update-account.md)|[account](../resources/account.md)|Update the properties of an account object.|
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read the properties and relationships of an [account](../resources/account.md) object.|
|[List journalLines](../api/journal-list-journallines.md)|[journalLine](../resources/journalline.md) collection|Get the journalLines from the journalLines navigation property.|
|[Create journalLines](../api/journal-post-journallines.md)|[journalLine](../resources/journalline.md)|Create a new journalLines object.|
|[Delete journalLines](../api/journal-delete-journallines.md)|None|Delete a [journalLine](../resources/journalline.md) object.|
|[Update journalLines](../api/journal-update-journallines.md)|[journalLine](../resources/journalline.md)|Update the properties of a journalLines object.|
|[Get journalLine](../api/journalline-get.md)|[journalLine](../resources/journalline.md)|Read the properties and relationships of a [journalLine](../resources/journalline.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|balancingAccountId|Guid|**TODO: Add Description**|
|balancingAccountNumber|String|**TODO: Add Description**|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)|**TODO: Add Description**|
|journalLines|[journalLine](../resources/journalline.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.journal",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.journal",
  "id": "String (identifier)",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "balancingAccountId": "Guid",
  "balancingAccountNumber": "String"
}
```

