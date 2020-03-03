---
title: "office365ActivationsUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# office365ActivationsUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365ActivationsUserCountses](../api/office365activationsusercounts-list.md)|[office365ActivationsUserCounts](../resources/office365ActivationsUserCounts.md) collection|List properties and relationships of the [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) objects.|
|[Get office365ActivationsUserCounts](../api/office365activationsusercounts-get.md)|[office365ActivationsUserCounts](../resources/office365ActivationsUserCounts.md)|Read properties and relationships of the [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.|
|[Create office365ActivationsUserCounts](../api/office365activationsusercounts-create.md)|[office365ActivationsUserCounts](../resources/office365ActivationsUserCounts.md)|Create a new [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.|
|[Delete office365ActivationsUserCounts](../api/office365activationsusercounts-delete.md)|None|Deletes a [office365ActivationsUserCounts](../resources/office365activationsusercounts.md).|
|[Update office365ActivationsUserCounts](../api/office365activationsusercounts-update.md)|[office365ActivationsUserCounts](../resources/office365ActivationsUserCounts.md)|Update the properties of a [office365ActivationsUserCounts](../resources/office365activationsusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activated|Int64||
|assigned|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|productType|String||
|reportRefreshDate|Date||
|sharedComputerActivation|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365ActivationsUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "productType": "String",
  "assigned": 1024,
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```

