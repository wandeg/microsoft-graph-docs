---
title: "sharePointActivityPages resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sharePointActivityPages resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List sharePointActivityPageses](../api/sharepointactivitypages-list.md)|[sharePointActivityPages](../resources/sharePointActivityPages.md) collection|List properties and relationships of the [sharePointActivityPages](../resources/sharepointactivitypages.md) objects.|
|[Get sharePointActivityPages](../api/sharepointactivitypages-get.md)|[sharePointActivityPages](../resources/sharePointActivityPages.md)|Read properties and relationships of the [sharePointActivityPages](../resources/sharepointactivitypages.md) object.|
|[Create sharePointActivityPages](../api/sharepointactivitypages-create.md)|[sharePointActivityPages](../resources/sharePointActivityPages.md)|Create a new [sharePointActivityPages](../resources/sharepointactivitypages.md) object.|
|[Delete sharePointActivityPages](../api/sharepointactivitypages-delete.md)|None|Deletes a [sharePointActivityPages](../resources/sharepointactivitypages.md).|
|[Update sharePointActivityPages](../api/sharepointactivitypages-update.md)|[sharePointActivityPages](../resources/sharePointActivityPages.md)|Update the properties of a [sharePointActivityPages](../resources/sharepointactivitypages.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|visitedPageCount|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.sharePointActivityPages",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharePointActivityPages",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "visitedPageCount": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

