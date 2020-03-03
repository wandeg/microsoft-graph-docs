---
title: "office365GroupsActivityGroupCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# office365GroupsActivityGroupCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365GroupsActivityGroupCountses](../api/office365groupsactivitygroupcounts-list.md)|[office365GroupsActivityGroupCounts](../resources/office365GroupsActivityGroupCounts.md) collection|List properties and relationships of the [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) objects.|
|[Get office365GroupsActivityGroupCounts](../api/office365groupsactivitygroupcounts-get.md)|[office365GroupsActivityGroupCounts](../resources/office365GroupsActivityGroupCounts.md)|Read properties and relationships of the [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object.|
|[Create office365GroupsActivityGroupCounts](../api/office365groupsactivitygroupcounts-create.md)|[office365GroupsActivityGroupCounts](../resources/office365GroupsActivityGroupCounts.md)|Create a new [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object.|
|[Delete office365GroupsActivityGroupCounts](../api/office365groupsactivitygroupcounts-delete.md)|None|Deletes a [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md).|
|[Update office365GroupsActivityGroupCounts](../api/office365groupsactivitygroupcounts-update.md)|[office365GroupsActivityGroupCounts](../resources/office365GroupsActivityGroupCounts.md)|Update the properties of a [office365GroupsActivityGroupCounts](../resources/office365groupsactivitygroupcounts.md) object.|

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
  "@odata.type": "microsoft.graph.office365GroupsActivityGroupCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365GroupsActivityGroupCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

