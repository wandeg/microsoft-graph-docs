---
title: "timeOffRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# timeOffRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [scheduleChangeRequest](../resources/schedulechangerequest.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[approve](../api/timeoffrequest-approve.md)|None|**TODO: Add Description**|
|[decline](../api/timeoffrequest-decline.md)|None|**TODO: Add Description**|
|[List timeOffRequests](../api/schedule-list-timeoffrequests.md)|[timeOffRequest](../resources/timeoffrequest.md) collection|Get the timeOffRequests from the timeOffRequests navigation property.|
|[Create timeOffRequests](../api/schedule-post-timeoffrequests.md)|[timeOffRequest](../resources/timeoffrequest.md)|Create a new timeOffRequests object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|scheduleChangeRequestActor|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|managerActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|state|scheduleChangeState|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|
|timeOffReasonId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

