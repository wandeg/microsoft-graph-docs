---
title: "yammerGroupsActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# yammerGroupsActivityCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List yammerGroupsActivityCountses](../api/yammergroupsactivitycounts-list.md)|[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) collection|List properties and relationships of the [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) objects.|
|[Get yammerGroupsActivityCounts](../api/yammergroupsactivitycounts-get.md)|[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)|Read properties and relationships of the [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object.|
|[Create yammerGroupsActivityCounts](../api/yammergroupsactivitycounts-create.md)|[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)|Create a new [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object.|
|[Delete yammerGroupsActivityCounts](../api/yammergroupsactivitycounts-delete.md)|None|Deletes a [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md).|
|[Update yammerGroupsActivityCounts](../api/yammergroupsactivitycounts-update.md)|[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)|Update the properties of a [yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|liked|Int64||
|posted|Int64||
|read|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "liked": 1024,
  "posted": 1024,
  "read": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

