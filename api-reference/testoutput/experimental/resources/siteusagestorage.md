---
title: "siteUsageStorage resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# siteUsageStorage resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List siteUsageStorages](../api/siteusagestorage-list.md)|[siteUsageStorage](../resources/siteusagestorage.md) collection|List properties and relationships of the [siteUsageStorage](../resources/siteusagestorage.md) objects.|
|[Get siteUsageStorage](../api/siteusagestorage-get.md)|[siteUsageStorage](../resources/siteusagestorage.md)|Read properties and relationships of the [siteUsageStorage](../resources/siteusagestorage.md) object.|
|[Create siteUsageStorage](../api/siteusagestorage-create.md)|[siteUsageStorage](../resources/siteusagestorage.md)|Create a new [siteUsageStorage](../resources/siteusagestorage.md) object.|
|[Delete siteUsageStorage](../api/siteusagestorage-delete.md)|None|Deletes a [siteUsageStorage](../resources/siteusagestorage.md).|
|[Update siteUsageStorage](../api/siteusagestorage-update.md)|[siteUsageStorage](../resources/siteusagestorage.md)|Update the properties of a [siteUsageStorage](../resources/siteusagestorage.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|siteType|String||
|storageUsedInBytes|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteUsageStorage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.siteUsageStorage",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "siteType": "String",
  "storageUsedInBytes": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

