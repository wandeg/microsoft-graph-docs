---
title: "skypeForBusinessParticipantActivityUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# skypeForBusinessParticipantActivityUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessParticipantActivityUserCountses](../api/skypeforbusinessparticipantactivityusercounts-list.md)|[skypeForBusinessParticipantActivityUserCounts](../resources/skypeForBusinessParticipantActivityUserCounts.md) collection|List properties and relationships of the [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) objects.|
|[Get skypeForBusinessParticipantActivityUserCounts](../api/skypeforbusinessparticipantactivityusercounts-get.md)|[skypeForBusinessParticipantActivityUserCounts](../resources/skypeForBusinessParticipantActivityUserCounts.md)|Read properties and relationships of the [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) object.|
|[Create skypeForBusinessParticipantActivityUserCounts](../api/skypeforbusinessparticipantactivityusercounts-create.md)|[skypeForBusinessParticipantActivityUserCounts](../resources/skypeForBusinessParticipantActivityUserCounts.md)|Create a new [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) object.|
|[Delete skypeForBusinessParticipantActivityUserCounts](../api/skypeforbusinessparticipantactivityusercounts-delete.md)|None|Deletes a [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md).|
|[Update skypeForBusinessParticipantActivityUserCounts](../api/skypeforbusinessparticipantactivityusercounts-update.md)|[skypeForBusinessParticipantActivityUserCounts](../resources/skypeForBusinessParticipantActivityUserCounts.md)|Update the properties of a [skypeForBusinessParticipantActivityUserCounts](../resources/skypeforbusinessparticipantactivityusercounts.md) object.|

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
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessParticipantActivityUserCounts",
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

