---
title: "skypeForBusinessParticipantActivityCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessParticipantActivityCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessParticipantActivityCountses](../api/skypeforbusinessparticipantactivitycounts-list.md)|[skypeForBusinessParticipantActivityCounts](../resources/skypeForBusinessParticipantActivityCounts.md) collection|List properties and relationships of the [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) objects.|
|[Get skypeForBusinessParticipantActivityCounts](../api/skypeforbusinessparticipantactivitycounts-get.md)|[skypeForBusinessParticipantActivityCounts](../resources/skypeForBusinessParticipantActivityCounts.md)|Read properties and relationships of the [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) object.|
|[Create skypeForBusinessParticipantActivityCounts](../api/skypeforbusinessparticipantactivitycounts-create.md)|[skypeForBusinessParticipantActivityCounts](../resources/skypeForBusinessParticipantActivityCounts.md)|Create a new [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) object.|
|[Delete skypeForBusinessParticipantActivityCounts](../api/skypeforbusinessparticipantactivitycounts-delete.md)|None|Deletes a [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md).|
|[Update skypeForBusinessParticipantActivityCounts](../api/skypeforbusinessparticipantactivitycounts-update.md)|[skypeForBusinessParticipantActivityCounts](../resources/skypeForBusinessParticipantActivityCounts.md)|Update the properties of a [skypeForBusinessParticipantActivityCounts](../resources/skypeforbusinessparticipantactivitycounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appSharing|Int64||
|audioVideo|Int64||
|dialInOut3rdParty|Int64||
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
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessParticipantActivityCounts",
  "id": "String (identifier)",
  "im": 1024,
  "audioVideo": 1024,
  "appSharing": 1024,
  "web": 1024,
  "dialInOut3rdParty": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

