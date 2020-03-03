---
title: "mailboxUsageMailboxCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mailboxUsageMailboxCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailboxUsageMailboxCountses](../api/mailboxusagemailboxcounts-list.md)|[mailboxUsageMailboxCounts](../resources/mailboxUsageMailboxCounts.md) collection|List properties and relationships of the [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) objects.|
|[Get mailboxUsageMailboxCounts](../api/mailboxusagemailboxcounts-get.md)|[mailboxUsageMailboxCounts](../resources/mailboxUsageMailboxCounts.md)|Read properties and relationships of the [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.|
|[Create mailboxUsageMailboxCounts](../api/mailboxusagemailboxcounts-create.md)|[mailboxUsageMailboxCounts](../resources/mailboxUsageMailboxCounts.md)|Create a new [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.|
|[Delete mailboxUsageMailboxCounts](../api/mailboxusagemailboxcounts-delete.md)|None|Deletes a [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md).|
|[Update mailboxUsageMailboxCounts](../api/mailboxusagemailboxcounts-update.md)|[mailboxUsageMailboxCounts](../resources/mailboxUsageMailboxCounts.md)|Update the properties of a [mailboxUsageMailboxCounts](../resources/mailboxusagemailboxcounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|active|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|total|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailboxUsageMailboxCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailboxUsageMailboxCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

