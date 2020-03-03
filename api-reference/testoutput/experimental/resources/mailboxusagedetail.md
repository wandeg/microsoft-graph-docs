---
title: "mailboxUsageDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# mailboxUsageDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List mailboxUsageDetails](../api/mailboxusagedetail-list.md)|[mailboxUsageDetail](../resources/mailboxusagedetail.md) collection|List properties and relationships of the [mailboxUsageDetail](../resources/mailboxusagedetail.md) objects.|
|[Get mailboxUsageDetail](../api/mailboxusagedetail-get.md)|[mailboxUsageDetail](../resources/mailboxusagedetail.md)|Read properties and relationships of the [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.|
|[Create mailboxUsageDetail](../api/mailboxusagedetail-create.md)|[mailboxUsageDetail](../resources/mailboxusagedetail.md)|Create a new [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.|
|[Delete mailboxUsageDetail](../api/mailboxusagedetail-delete.md)|None|Deletes a [mailboxUsageDetail](../resources/mailboxusagedetail.md).|
|[Update mailboxUsageDetail](../api/mailboxusagedetail-update.md)|[mailboxUsageDetail](../resources/mailboxusagedetail.md)|Update the properties of a [mailboxUsageDetail](../resources/mailboxusagedetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDate|Date||
|deletedDate|Date||
|deletedItemCount|Int64||
|deletedItemSizeInBytes|Int64||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|issueWarningQuotaInBytes|Int64||
|itemCount|Int64||
|lastActivityDate|Date||
|prohibitSendQuotaInBytes|Int64||
|prohibitSendReceiveQuotaInBytes|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|storageUsedInBytes|Int64||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailboxUsageDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailboxUsageDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "createdDate": "Date",
  "lastActivityDate": "Date",
  "itemCount": 1024,
  "storageUsedInBytes": 1024,
  "deletedItemCount": 1024,
  "deletedItemSizeInBytes": 1024,
  "issueWarningQuotaInBytes": 1024,
  "prohibitSendQuotaInBytes": 1024,
  "prohibitSendReceiveQuotaInBytes": 1024,
  "reportPeriod": "String"
}
```

