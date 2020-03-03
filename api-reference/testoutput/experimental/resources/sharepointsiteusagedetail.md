---
title: "sharePointSiteUsageDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharePointSiteUsageDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointSiteUsageDetails](../api/sharepointsiteusagedetail-list.md)|[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) collection|List properties and relationships of the [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) objects.|
|[Get sharePointSiteUsageDetail](../api/sharepointsiteusagedetail-get.md)|[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)|Read properties and relationships of the [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object.|
|[Create sharePointSiteUsageDetail](../api/sharepointsiteusagedetail-create.md)|[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)|Create a new [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object.|
|[Delete sharePointSiteUsageDetail](../api/sharepointsiteusagedetail-delete.md)|None|Deletes a [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md).|
|[Update sharePointSiteUsageDetail](../api/sharepointsiteusagedetail-update.md)|[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)|Update the properties of a [sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md) object.|

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
|pageViewCount|Int64||
|reportPeriod|String||
|reportRefreshDate|Date||
|rootWebTemplate|String||
|siteId|Guid||
|siteUrl|String||
|storageAllocatedInBytes|Int64||
|storageUsedInBytes|Int64||
|visitedPageCount|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointSiteUsageDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteId": "Guid",
  "siteUrl": "String",
  "ownerDisplayName": "String",
  "ownerPrincipalName": "String",
  "isDeleted": true,
  "lastActivityDate": "Date",
  "fileCount": 1024,
  "activeFileCount": 1024,
  "pageViewCount": 1024,
  "visitedPageCount": 1024,
  "storageUsedInBytes": 1024,
  "storageAllocatedInBytes": 1024,
  "rootWebTemplate": "String",
  "reportPeriod": "String"
}
```

