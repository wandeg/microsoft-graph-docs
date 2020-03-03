---
title: "timeOff resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# timeOff resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get timeOff](../api/timeoff-get.md)|[timeOff](../resources/timeOff.md)|Read properties and relationships of the [timeOff](../resources/timeoff.md) object.|
|[Delete timeOff](../api/timeoff-delete.md)|None|Deletes a [timeOff](../resources/timeoff.md).|
|[Update timeOff](../api/timeoff-update.md)|[timeOff](../resources/timeOff.md)|Update the properties of a [timeOff](../resources/timeoff.md) object.|
|[List timesOff](../api/schedule-list-timesoff.md)|[timeOff](../resources/timeOff.md) collection|Get the timeOffs from the timesOff navigation property.|
|[Add timesOff](../api/schedule-post-timesoff.md)|[timeOff](../resources/timeOff.md)|Add timesOff by posting to the timesOff collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|draftTimeOff|[timeOffItem](../resources/timeOffItem.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|sharedTimeOff|[timeOffItem](../resources/timeOffItem.md)||
|userId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOff",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeOff",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "String"
}
```

