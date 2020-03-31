---
title: "timeOffRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# timeOffRequest resource type


Namespace: microsoft.graph




Inherits from [scheduleChangeRequest](../resources/schedulechangerequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get timeOffRequest](../api/timeoffrequest-get.md)|[timeOffRequest](../resources/timeoffrequest.md)|Read properties and relationships of the [timeOffRequest](../resources/timeoffrequest.md) object.|
|[Update timeOffRequest](../api/timeoffrequest-update.md)|[timeOffRequest](../resources/timeoffrequest.md)|Update the properties of a [timeOffRequest](../resources/timeoffrequest.md) object.|
|[approve](../api/timeoffrequest-approve.md)|None||
|[decline](../api/timeoffrequest-decline.md)|None||
|[List timeOffRequests](../api/schedule-list-timeoffrequests.md)|[timeOffRequest](../resources/timeoffrequest.md) collection|Get the timeOffRequests from the timeOffRequests navigation property.|
|[Add timeOffRequests](../api/schedule-post-timeoffrequests.md)|[timeOffRequest](../resources/timeoffrequest.md)|Add timeOffRequests by posting to the timeOffRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|endDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|managerActionDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|startDateTime|DateTimeOffset||
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|
|timeOffReasonId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeOffRequest",
  "baseType": "microsoft.graph.scheduleChangeRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.timeOffRequest",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "assignedTo": "String",
  "state": "String",
  "senderMessage": "String",
  "senderDateTime": "String (timestamp)",
  "managerActionMessage": "String",
  "managerActionDateTime": "String (timestamp)",
  "senderUserId": "String",
  "managerUserId": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "timeOffReasonId": "String"
}
```

