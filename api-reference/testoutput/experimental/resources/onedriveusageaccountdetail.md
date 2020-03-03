---
title: "oneDriveUsageAccountDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# oneDriveUsageAccountDetail resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List oneDriveUsageAccountDetails](../api/onedriveusageaccountdetail-list.md)|[oneDriveUsageAccountDetail](../resources/oneDriveUsageAccountDetail.md) collection|List properties and relationships of the [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) objects.|
|[Get oneDriveUsageAccountDetail](../api/onedriveusageaccountdetail-get.md)|[oneDriveUsageAccountDetail](../resources/oneDriveUsageAccountDetail.md)|Read properties and relationships of the [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) object.|
|[Create oneDriveUsageAccountDetail](../api/onedriveusageaccountdetail-create.md)|[oneDriveUsageAccountDetail](../resources/oneDriveUsageAccountDetail.md)|Create a new [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) object.|
|[Delete oneDriveUsageAccountDetail](../api/onedriveusageaccountdetail-delete.md)|None|Deletes a [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md).|
|[Update oneDriveUsageAccountDetail](../api/onedriveusageaccountdetail-update.md)|[oneDriveUsageAccountDetail](../resources/oneDriveUsageAccountDetail.md)|Update the properties of a [oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeFileCount|Int64||
|fileCount|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|ownerDisplayName|String||
|ownerPrincipalName|String||
|reportPeriod|String||
|reportRefreshDate|Date||
|siteUrl|String||
|storageAllocatedInBytes|Int64||
|storageUsedInBytes|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oneDriveUsageAccountDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "reportPeriod": "String"
}
```

