---
title: "office365GroupsActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# office365GroupsActivityCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365GroupsActivityCountses](../api/office365groupsactivitycounts-list.md)|[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) collection|List properties and relationships of the [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) objects.|
|[Get office365GroupsActivityCounts](../api/office365groupsactivitycounts-get.md)|[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)|Read properties and relationships of the [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object.|
|[Create office365GroupsActivityCounts](../api/office365groupsactivitycounts-create.md)|[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)|Create a new [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object.|
|[Delete office365GroupsActivityCounts](../api/office365groupsactivitycounts-delete.md)|None|Deletes a [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md).|
|[Update office365GroupsActivityCounts](../api/office365groupsactivitycounts-update.md)|[office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md)|Update the properties of a [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exchangeEmailsReceived|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|yammerMessagesLiked|Int64||
|yammerMessagesPosted|Int64||
|yammerMessagesRead|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365GroupsActivityCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "exchangeEmailsReceived": 1024,
  "yammerMessagesPosted": 1024,
  "yammerMessagesRead": 1024,
  "yammerMessagesLiked": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

