---
title: "timeOffReason resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# timeOffReason resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [changeTrackedEntity](../resources/changetrackedentity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get timeOffReason](../api/timeoffreason-get.md)|[timeOffReason](../resources/timeoffreason.md)|Read the properties and relationships of a [timeOffReason](../resources/timeoffreason.md) object.|
|[Update timeOffReason](../api/timeoffreason-update.md)|[timeOffReason](../resources/timeoffreason.md)|Update the properties of a [timeOffReason](../resources/timeoffreason.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|displayName|String|**TODO: Add Description**|
|iconType|timeOffReasonIconType|**TODO: Add Description**. Possible values are: `none`, `car`, `calendar`, `running`, `plane`, `firstAid`, `doctor`, `notWorking`, `clock`, `juryDuty`, `globe`, `cup`, `phone`, `weather`, `umbrella`, `piggyBank`, `dog`, `cake`, `trafficCone`, `pin`, `sunny`, `unknownFutureValue`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isActive|Boolean|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|

## Relationships
None

## JSON representation
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

