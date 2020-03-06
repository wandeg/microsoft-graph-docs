---
title: "journal resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# journal resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get journal](../api/journal-get.md)|[journal](../resources/journal.md)|Read properties and relationships of the [journal](../resources/journal.md) object.|
|[Update journal](../api/journal-update.md)|[journal](../resources/journal.md)|Update the properties of a [journal](../resources/journal.md) object.|
|[post](../api/journal-post.md)|None||
|[Get account](../api/account-get.md)|[account](../resources/account.md)|Read properties and relationships of the [account](../resources/account.md) object.|
|[List journalLines](../api/journal-list-journallines.md)|[journalLine](../resources/journalline.md) collection|Get the journalLines from the journalLines navigation property.|
|[Add journalLines](../api/journal-post-journallines.md)|[journalLine](../resources/journalline.md)|Add journalLines by posting to the journalLines collection.|
|[List journals](../api/company-list-journals.md)|[journal](../resources/journal.md) collection|Get the journals from the journals navigation property.|
|[Add journals](../api/company-post-journals.md)|[journal](../resources/journal.md)|Add journals by posting to the journals collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|balancingAccountId|Guid||
|balancingAccountNumber|String||
|code|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)||
|journalLines|[journalLine](../resources/journalline.md) collection||

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

