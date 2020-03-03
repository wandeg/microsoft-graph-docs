---
title: "timeOffReason resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# timeOffReason resource type




Inherits from [changeTrackedEntity](../resources/changeTrackedEntity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get timeOffReason](../api/timeoffreason-get.md)|[timeOffReason](../resources/timeOffReason.md)|Read properties and relationships of the [timeOffReason](../resources/timeoffreason.md) object.|
|[Delete timeOffReason](../api/timeoffreason-delete.md)|None|Deletes a [timeOffReason](../resources/timeoffreason.md).|
|[Update timeOffReason](../api/timeoffreason-update.md)|[timeOffReason](../resources/timeOffReason.md)|Update the properties of a [timeOffReason](../resources/timeoffreason.md) object.|
|[List timeOffReasons](../api/schedule-list-timeoffreasons.md)|[timeOffReason](../resources/timeOffReason.md) collection|Get the timeOffReasons from the timeOffReasons navigation property.|
|[Add timeOffReasons](../api/schedule-post-timeoffreasons.md)|[timeOffReason](../resources/timeOffReason.md)|Add timeOffReasons by posting to the timeOffReasons collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|displayName|String||
|iconType|Enumeration|. Possible values are: `none`, `car`, `calendar`, `running`, `plane`, `firstAid`, `doctor`, `notWorking`, `clock`, `juryDuty`, `globe`, `cup`, `phone`, `weather`, `umbrella`, `piggyBank`, `dog`, `cake`, `trafficCone`, `pin`, `sunny`, `unknownFutureValue`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isActive|Boolean||
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffReason",
  "baseType": "microsoft.graph.changeTrackedEntity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeOffReason",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "displayName": "String",
  "iconType": "String",
  "isActive": true
}
```

