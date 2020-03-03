---
title: "oneDriveUsageFileCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# oneDriveUsageFileCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List oneDriveUsageFileCountses](../api/onedriveusagefilecounts-list.md)|[oneDriveUsageFileCounts](../resources/oneDriveUsageFileCounts.md) collection|List properties and relationships of the [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) objects.|
|[Get oneDriveUsageFileCounts](../api/onedriveusagefilecounts-get.md)|[oneDriveUsageFileCounts](../resources/oneDriveUsageFileCounts.md)|Read properties and relationships of the [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) object.|
|[Create oneDriveUsageFileCounts](../api/onedriveusagefilecounts-create.md)|[oneDriveUsageFileCounts](../resources/oneDriveUsageFileCounts.md)|Create a new [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) object.|
|[Delete oneDriveUsageFileCounts](../api/onedriveusagefilecounts-delete.md)|None|Deletes a [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md).|
|[Update oneDriveUsageFileCounts](../api/onedriveusagefilecounts-update.md)|[oneDriveUsageFileCounts](../resources/oneDriveUsageFileCounts.md)|Update the properties of a [oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md) object.|

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
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oneDriveUsageFileCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

