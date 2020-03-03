---
title: "skypeForBusinessParticipantActivityMinuteCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# skypeForBusinessParticipantActivityMinuteCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List skypeForBusinessParticipantActivityMinuteCountses](../api/skypeforbusinessparticipantactivityminutecounts-list.md)|[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) collection|List properties and relationships of the [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) objects.|
|[Get skypeForBusinessParticipantActivityMinuteCounts](../api/skypeforbusinessparticipantactivityminutecounts-get.md)|[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)|Read properties and relationships of the [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) object.|
|[Create skypeForBusinessParticipantActivityMinuteCounts](../api/skypeforbusinessparticipantactivityminutecounts-create.md)|[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)|Create a new [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) object.|
|[Delete skypeForBusinessParticipantActivityMinuteCounts](../api/skypeforbusinessparticipantactivityminutecounts-delete.md)|None|Deletes a [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md).|
|[Update skypeForBusinessParticipantActivityMinuteCounts](../api/skypeforbusinessparticipantactivityminutecounts-update.md)|[skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md)|Update the properties of a [skypeForBusinessParticipantActivityMinuteCounts](../resources/skypeforbusinessparticipantactivityminutecounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|audiovideo|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
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
  "@odata.type": "microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.skypeForBusinessParticipantActivityMinuteCounts",
  "id": "String (identifier)",
  "audiovideo": 1024,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "String"
}
```

