---
title: "office365GroupsActivityFileCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# office365GroupsActivityFileCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365GroupsActivityFileCountses](../api/office365groupsactivityfilecounts-list.md)|[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) collection|List properties and relationships of the [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) objects.|
|[Get office365GroupsActivityFileCounts](../api/office365groupsactivityfilecounts-get.md)|[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)|Read properties and relationships of the [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) object.|
|[Create office365GroupsActivityFileCounts](../api/office365groupsactivityfilecounts-create.md)|[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)|Create a new [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) object.|
|[Delete office365GroupsActivityFileCounts](../api/office365groupsactivityfilecounts-delete.md)|None|Deletes a [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md).|
|[Update office365GroupsActivityFileCounts](../api/office365groupsactivityfilecounts-update.md)|[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)|Update the properties of a [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) object.|

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
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365GroupsActivityFileCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "total": 1024,
  "active": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

