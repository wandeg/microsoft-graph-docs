---
title: "sharePointSiteUsageSiteCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sharePointSiteUsageSiteCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointSiteUsageSiteCountses](../api/sharepointsiteusagesitecounts-list.md)|[sharePointSiteUsageSiteCounts](../resources/sharePointSiteUsageSiteCounts.md) collection|List properties and relationships of the [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) objects.|
|[Get sharePointSiteUsageSiteCounts](../api/sharepointsiteusagesitecounts-get.md)|[sharePointSiteUsageSiteCounts](../resources/sharePointSiteUsageSiteCounts.md)|Read properties and relationships of the [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) object.|
|[Create sharePointSiteUsageSiteCounts](../api/sharepointsiteusagesitecounts-create.md)|[sharePointSiteUsageSiteCounts](../resources/sharePointSiteUsageSiteCounts.md)|Create a new [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) object.|
|[Delete sharePointSiteUsageSiteCounts](../api/sharepointsiteusagesitecounts-delete.md)|None|Deletes a [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md).|
|[Update sharePointSiteUsageSiteCounts](../api/sharepointsiteusagesitecounts-update.md)|[sharePointSiteUsageSiteCounts](../resources/sharePointSiteUsageSiteCounts.md)|Update the properties of a [sharePointSiteUsageSiteCounts](../resources/sharepointsiteusagesitecounts.md) object.|

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
  "@odata.type": "microsoft.graph.sharePointSiteUsageSiteCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointSiteUsageSiteCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteType": "String",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

