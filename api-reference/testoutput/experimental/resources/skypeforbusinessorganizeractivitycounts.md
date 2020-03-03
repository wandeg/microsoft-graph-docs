---
title: "skypeForBusinessOrganizerActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessOrganizerActivityCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessOrganizerActivityCountses](../api/skypeforbusinessorganizeractivitycounts-list.md)|[skypeForBusinessOrganizerActivityCounts](../resources/skypeForBusinessOrganizerActivityCounts.md) collection|List properties and relationships of the [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) objects.|
|[Get skypeForBusinessOrganizerActivityCounts](../api/skypeforbusinessorganizeractivitycounts-get.md)|[skypeForBusinessOrganizerActivityCounts](../resources/skypeForBusinessOrganizerActivityCounts.md)|Read properties and relationships of the [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) object.|
|[Create skypeForBusinessOrganizerActivityCounts](../api/skypeforbusinessorganizeractivitycounts-create.md)|[skypeForBusinessOrganizerActivityCounts](../resources/skypeForBusinessOrganizerActivityCounts.md)|Create a new [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) object.|
|[Delete skypeForBusinessOrganizerActivityCounts](../api/skypeforbusinessorganizeractivitycounts-delete.md)|None|Deletes a [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md).|
|[Update skypeForBusinessOrganizerActivityCounts](../api/skypeforbusinessorganizeractivitycounts-update.md)|[skypeForBusinessOrganizerActivityCounts](../resources/skypeForBusinessOrganizerActivityCounts.md)|Update the properties of a [skypeForBusinessOrganizerActivityCounts](../resources/skypeforbusinessorganizeractivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appSharing|Int64||
|audioVideo|Int64||
|dialInOut3rdParty|Int64||
|dialInOutMicrosoft|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|web|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.skypeForBusinessOrganizerActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessOrganizerActivityCounts",
  "id": "String (identifier)",
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "dialInOutMicrosoft": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

