---
title: "swapShiftsChangeRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# swapShiftsChangeRequest resource type




Inherits from [offerShiftRequest](../resources/offerShiftRequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get swapShiftsChangeRequest](../api/swapshiftschangerequest-get.md)|[swapShiftsChangeRequest](../resources/swapShiftsChangeRequest.md)|Read properties and relationships of the [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[Delete swapShiftsChangeRequest](../api/swapshiftschangerequest-delete.md)|None|Deletes a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md).|
|[Update swapShiftsChangeRequest](../api/swapshiftschangerequest-update.md)|[swapShiftsChangeRequest](../resources/swapShiftsChangeRequest.md)|Update the properties of a [swapShiftsChangeRequest](../resources/swapshiftschangerequest.md) object.|
|[List swapShiftsChangeRequests](../api/schedule-list-swapshiftschangerequests.md)|[swapShiftsChangeRequest](../resources/swapShiftsChangeRequest.md) collection|Get the swapShiftsChangeRequests from the swapShiftsChangeRequests navigation property.|
|[Add swapShiftsChangeRequests](../api/schedule-post-swapshiftschangerequests.md)|[swapShiftsChangeRequest](../resources/swapShiftsChangeRequest.md)|Add swapShiftsChangeRequests by posting to the swapShiftsChangeRequests collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|Enumeration| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [changeTrackedEntity](../resources/changeTrackedEntity.md)|
|managerActionDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|managerActionMessage|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|managerUserId|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|recipientActionDateTime|DateTimeOffset| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|recipientActionMessage|String| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|recipientShiftId|String||
|recipientUserId|String| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|senderShiftId|String| Inherited from [offerShiftRequest](../resources/offerShiftRequest.md)|
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
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

