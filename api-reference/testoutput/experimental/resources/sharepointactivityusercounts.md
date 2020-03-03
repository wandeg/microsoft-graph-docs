---
title: "sharePointActivityUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# sharePointActivityUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointActivityUserCountses](../api/sharepointactivityusercounts-list.md)|[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) collection|List properties and relationships of the [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) objects.|
|[Get sharePointActivityUserCounts](../api/sharepointactivityusercounts-get.md)|[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)|Read properties and relationships of the [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) object.|
|[Create sharePointActivityUserCounts](../api/sharepointactivityusercounts-create.md)|[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)|Create a new [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) object.|
|[Delete sharePointActivityUserCounts](../api/sharepointactivityusercounts-delete.md)|None|Deletes a [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md).|
|[Update sharePointActivityUserCounts](../api/sharepointactivityusercounts-update.md)|[sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md)|Update the properties of a [sharePointActivityUserCounts](../resources/sharepointactivityusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|sharedExternally|Int64||
|sharedInternally|Int64||
|synced|Int64||
|viewedOrEdited|Int64||
|visitedPage|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharePointActivityUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointActivityUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "visitedPage": 1024,
  "viewedOrEdited": 1024,
  "synced": 1024,
  "sharedInternally": 1024,
  "sharedExternally": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

