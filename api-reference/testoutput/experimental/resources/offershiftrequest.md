---
title: "offerShiftRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# offerShiftRequest resource type




Inherits from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get offerShiftRequest](../api/offershiftrequest-get.md)|[offerShiftRequest](../resources/offerShiftRequest.md)|Read properties and relationships of the [offerShiftRequest](../resources/offershiftrequest.md) object.|
|[Delete offerShiftRequest](../api/offershiftrequest-delete.md)|None|Deletes a [offerShiftRequest](../resources/offershiftrequest.md).|
|[Update offerShiftRequest](../api/offershiftrequest-update.md)|[offerShiftRequest](../resources/offerShiftRequest.md)|Update the properties of a [offerShiftRequest](../resources/offershiftrequest.md) object.|
|[approve](../api/offershiftrequest-approve.md)|None||
|[decline](../api/offershiftrequest-decline.md)|None||
|[List offerShiftRequests](../api/schedule-list-offershiftrequests.md)|[offerShiftRequest](../resources/offerShiftRequest.md) collection|Get the offerShiftRequests from the offerShiftRequests navigation property.|
|[Add offerShiftRequests](../api/schedule-post-offershiftrequests.md)|[offerShiftRequest](../resources/offerShiftRequest.md)|Add offerShiftRequests by posting to the offerShiftRequests collection.|

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
|recipientActionDateTime|DateTimeOffset||
|recipientActionMessage|String||
|recipientUserId|String||
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|senderShiftId|String||
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md)|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/scheduleChangeRequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.offerShiftRequest",
  "baseType": "microsoft.graph.scheduleChangeRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.offerShiftRequest",
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
  "recipientUserId": "String"
}
```

