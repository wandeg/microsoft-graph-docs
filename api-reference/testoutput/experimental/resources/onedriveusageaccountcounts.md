---
title: "oneDriveUsageAccountCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# oneDriveUsageAccountCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List oneDriveUsageAccountCountses](../api/onedriveusageaccountcounts-list.md)|[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) collection|List properties and relationships of the [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) objects.|
|[Get oneDriveUsageAccountCounts](../api/onedriveusageaccountcounts-get.md)|[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)|Read properties and relationships of the [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) object.|
|[Create oneDriveUsageAccountCounts](../api/onedriveusageaccountcounts-create.md)|[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)|Create a new [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) object.|
|[Delete oneDriveUsageAccountCounts](../api/onedriveusageaccountcounts-delete.md)|None|Deletes a [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md).|
|[Update oneDriveUsageAccountCounts](../api/onedriveusageaccountcounts-update.md)|[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)|Update the properties of a [oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|active|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|siteType|String||
|total|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oneDriveUsageAccountCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

