---
title: "yammerGroupsActivityGroupCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# yammerGroupsActivityGroupCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerGroupsActivityGroupCountses](../api/yammergroupsactivitygroupcounts-list.md)|[yammerGroupsActivityGroupCounts](../resources/yammerGroupsActivityGroupCounts.md) collection|List properties and relationships of the [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) objects.|
|[Get yammerGroupsActivityGroupCounts](../api/yammergroupsactivitygroupcounts-get.md)|[yammerGroupsActivityGroupCounts](../resources/yammerGroupsActivityGroupCounts.md)|Read properties and relationships of the [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object.|
|[Create yammerGroupsActivityGroupCounts](../api/yammergroupsactivitygroupcounts-create.md)|[yammerGroupsActivityGroupCounts](../resources/yammerGroupsActivityGroupCounts.md)|Create a new [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object.|
|[Delete yammerGroupsActivityGroupCounts](../api/yammergroupsactivitygroupcounts-delete.md)|None|Deletes a [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md).|
|[Update yammerGroupsActivityGroupCounts](../api/yammergroupsactivitygroupcounts-update.md)|[yammerGroupsActivityGroupCounts](../resources/yammerGroupsActivityGroupCounts.md)|Update the properties of a [yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|active|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|total|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityGroupCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

