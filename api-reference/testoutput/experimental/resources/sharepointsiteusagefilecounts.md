---
title: "sharePointSiteUsageFileCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharePointSiteUsageFileCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointSiteUsageFileCountses](../api/sharepointsiteusagefilecounts-list.md)|[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) collection|List properties and relationships of the [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) objects.|
|[Get sharePointSiteUsageFileCounts](../api/sharepointsiteusagefilecounts-get.md)|[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)|Read properties and relationships of the [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) object.|
|[Create sharePointSiteUsageFileCounts](../api/sharepointsiteusagefilecounts-create.md)|[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)|Create a new [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) object.|
|[Delete sharePointSiteUsageFileCounts](../api/sharepointsiteusagefilecounts-delete.md)|None|Deletes a [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md).|
|[Update sharePointSiteUsageFileCounts](../api/sharepointsiteusagefilecounts-update.md)|[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)|Update the properties of a [sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md) object.|

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
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointSiteUsageFileCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

