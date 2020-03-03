---
title: "sharePointSiteUsagePages resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharePointSiteUsagePages resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointSiteUsagePageses](../api/sharepointsiteusagepages-list.md)|[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) collection|List properties and relationships of the [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) objects.|
|[Get sharePointSiteUsagePages](../api/sharepointsiteusagepages-get.md)|[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)|Read properties and relationships of the [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) object.|
|[Create sharePointSiteUsagePages](../api/sharepointsiteusagepages-create.md)|[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)|Create a new [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) object.|
|[Delete sharePointSiteUsagePages](../api/sharepointsiteusagepages-delete.md)|None|Deletes a [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md).|
|[Update sharePointSiteUsagePages](../api/sharepointsiteusagepages-update.md)|[sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md)|Update the properties of a [sharePointSiteUsagePages](../resources/sharepointsiteusagepages.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|pageViewCount|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|siteType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharePointSiteUsagePages",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointSiteUsagePages",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteType": "String",
  "pageViewCount": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

