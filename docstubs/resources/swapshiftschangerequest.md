---
title: "swapShiftsChangeRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# swapShiftsChangeRequest resource type


Namespace: microsoft.graph




Inherits from [offerShiftRequest](../resources/offershiftrequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get swapShiftsChangeRequest](../api/swapshiftschangerequest-get.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Read properties and relationships of the [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[Update swapShiftsChangeRequest](../api/swapshiftschangerequest-update.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[List swapShiftsChangeRequests](../api/schedule-list-swapshiftschangerequests.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) collection|Get the swapShiftsChangeRequests from the swapShiftsChangeRequests navigation property.|
|[Add swapShiftsChangeRequests](../api/schedule-post-swapshiftschangerequests.md)|[swapShiftsChangeRequest](../resources/swapshiftschangerequest.md)|Add swapShiftsChangeRequests by posting to the swapShiftsChangeRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|managerActionDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|recipientActionDateTime|DateTimeOffset| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|recipientActionMessage|String| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|recipientShiftId|String||
|recipientUserId|String| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderShiftId|String| Inherited from [offerShiftRequest](../resources/offershiftrequest.md)|
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.swapShiftsChangeRequest",
  "baseType": "microsoft.graph.offerShiftRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.swapShiftsChangeRequest",
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
  "recipientActionMessage": "String",
  "recipientActionDateTime": "String (timestamp)",
  "senderShiftId": "String",
  "recipientUserId": "String",
  "recipientShiftId": "String"
}
```

