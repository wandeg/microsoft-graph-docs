---
title: "mailboxUsageQuotaStatusMailboxCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailboxUsageQuotaStatusMailboxCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailboxUsageQuotaStatusMailboxCountses](../api/mailboxusagequotastatusmailboxcounts-list.md)|[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) collection|List properties and relationships of the [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) objects.|
|[Get mailboxUsageQuotaStatusMailboxCounts](../api/mailboxusagequotastatusmailboxcounts-get.md)|[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)|Read properties and relationships of the [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object.|
|[Create mailboxUsageQuotaStatusMailboxCounts](../api/mailboxusagequotastatusmailboxcounts-create.md)|[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)|Create a new [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object.|
|[Delete mailboxUsageQuotaStatusMailboxCounts](../api/mailboxusagequotastatusmailboxcounts-delete.md)|None|Deletes a [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md).|
|[Update mailboxUsageQuotaStatusMailboxCounts](../api/mailboxusagequotastatusmailboxcounts-update.md)|[mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md)|Update the properties of a [mailboxUsageQuotaStatusMailboxCounts](../resources/mailboxusagequotastatusmailboxcounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|indeterminate|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|sendProhibited|Int64||
|sendReceiveProhibited|Int64||
|underLimit|Int64||
|warningIssued|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailboxUsageQuotaStatusMailboxCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailboxUsageQuotaStatusMailboxCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "underLimit": 1024,
  "warningIssued": 1024,
  "sendProhibited": 1024,
  "sendReceiveProhibited": 1024,
  "indeterminate": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

