---
title: "office365ActiveUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# office365ActiveUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365ActiveUserCountses](../api/office365activeusercounts-list.md)|[office365ActiveUserCounts](../resources/office365ActiveUserCounts.md) collection|List properties and relationships of the [office365ActiveUserCounts](../resources/office365activeusercounts.md) objects.|
|[Get office365ActiveUserCounts](../api/office365activeusercounts-get.md)|[office365ActiveUserCounts](../resources/office365ActiveUserCounts.md)|Read properties and relationships of the [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.|
|[Create office365ActiveUserCounts](../api/office365activeusercounts-create.md)|[office365ActiveUserCounts](../resources/office365ActiveUserCounts.md)|Create a new [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.|
|[Delete office365ActiveUserCounts](../api/office365activeusercounts-delete.md)|None|Deletes a [office365ActiveUserCounts](../resources/office365activeusercounts.md).|
|[Update office365ActiveUserCounts](../api/office365activeusercounts-update.md)|[office365ActiveUserCounts](../resources/office365ActiveUserCounts.md)|Update the properties of a [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exchange|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|office365|Int64||
|oneDrive|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|sharePoint|Int64||
|skypeForBusiness|Int64||
|teams|Int64||
|yammer|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365ActiveUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365ActiveUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "office365": 1024,
  "exchange": 1024,
  "oneDrive": 1024,
  "sharePoint": 1024,
  "skypeForBusiness": 1024,
  "yammer": 1024,
  "teams": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

