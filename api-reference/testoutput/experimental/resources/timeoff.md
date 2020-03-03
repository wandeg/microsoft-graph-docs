---
title: "timeOff resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# timeOff resource type


Namespace: microsoft.graph




Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List timeOffs](../api/timeoff-list.md)|[timeOff](../resources/timeoff.md) collection|List properties and relationships of the [timeOff](../resources/timeoff.md) objects.|
|[Get timeOff](../api/timeoff-get.md)|[timeOff](../resources/timeoff.md)|Read properties and relationships of the [timeOff](../resources/timeoff.md) object.|
|[Create timeOff](../api/timeoff-create.md)|[timeOff](../resources/timeoff.md)|Create a new [timeOff](../resources/timeoff.md) object.|
|[Delete timeOff](../api/timeoff-delete.md)|None|Deletes a [timeOff](../resources/timeoff.md).|
|[Update timeOff](../api/timeoff-update.md)|[timeOff](../resources/timeoff.md)|Update the properties of a [timeOff](../resources/timeoff.md) object.|
|[List timesOff](../api/schedule-list-timesoff.md)|[timeOff](../resources/timeoff.md) collection|Get the timeOffs from the timesOff navigation property.|
|[Add timesOff](../api/schedule-post-timesoff.md)|[timeOff](../resources/timeoff.md)|Add timesOff by posting to the timesOff collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|draftTimeOff|[timeOffItem](../resources/timeoffitem.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|sharedTimeOff|[timeOffItem](../resources/timeoffitem.md)||
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

