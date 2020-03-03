---
title: "skypeForBusinessPeerToPeerActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessPeerToPeerActivityCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessPeerToPeerActivityCountses](../api/skypeforbusinesspeertopeeractivitycounts-list.md)|[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) collection|List properties and relationships of the [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) objects.|
|[Get skypeForBusinessPeerToPeerActivityCounts](../api/skypeforbusinesspeertopeeractivitycounts-get.md)|[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)|Read properties and relationships of the [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) object.|
|[Create skypeForBusinessPeerToPeerActivityCounts](../api/skypeforbusinesspeertopeeractivitycounts-create.md)|[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)|Create a new [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) object.|
|[Delete skypeForBusinessPeerToPeerActivityCounts](../api/skypeforbusinesspeertopeeractivitycounts-delete.md)|None|Deletes a [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md).|
|[Update skypeForBusinessPeerToPeerActivityCounts](../api/skypeforbusinesspeertopeeractivitycounts-update.md)|[skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md)|Update the properties of a [skypeForBusinessPeerToPeerActivityCounts](../resources/skypeforbusinesspeertopeeractivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appSharing|Int64||
|audio|Int64||
|fileTransfer|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|video|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessPeerToPeerActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityCounts",
  "id": "String (identifier)",
  "im": 1024,
  "audio": 1024,
  "video": 1024,
  "appSharing": 1024,
  "fileTransfer": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

