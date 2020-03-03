---
title: "skypeForBusinessActivityUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessActivityUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessActivityUserCountses](../api/skypeforbusinessactivityusercounts-list.md)|[skypeForBusinessActivityUserCounts](../resources/skypeForBusinessActivityUserCounts.md) collection|List properties and relationships of the [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) objects.|
|[Get skypeForBusinessActivityUserCounts](../api/skypeforbusinessactivityusercounts-get.md)|[skypeForBusinessActivityUserCounts](../resources/skypeForBusinessActivityUserCounts.md)|Read properties and relationships of the [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object.|
|[Create skypeForBusinessActivityUserCounts](../api/skypeforbusinessactivityusercounts-create.md)|[skypeForBusinessActivityUserCounts](../resources/skypeForBusinessActivityUserCounts.md)|Create a new [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object.|
|[Delete skypeForBusinessActivityUserCounts](../api/skypeforbusinessactivityusercounts-delete.md)|None|Deletes a [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md).|
|[Update skypeForBusinessActivityUserCounts](../api/skypeforbusinessactivityusercounts-update.md)|[skypeForBusinessActivityUserCounts](../resources/skypeForBusinessActivityUserCounts.md)|Update the properties of a [skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|organized|Int64||
|participated|Int64||
|peerToPeer|Int64||
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
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessActivityUserCounts",
  "id": "String (identifier)",
  "peerToPeer": 1024,
  "organized": 1024,
  "participated": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

