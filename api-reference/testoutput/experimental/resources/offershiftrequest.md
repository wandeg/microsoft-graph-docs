---
title: "offerShiftRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# offerShiftRequest resource type


Namespace: microsoft.graph




Inherits from [scheduleChangeRequest](../resources/schedulechangerequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List offerShiftRequests](../api/offershiftrequest-list.md)|[offerShiftRequest](../resources/offershiftrequest.md) collection|List properties and relationships of the [offerShiftRequest](../resources/offershiftrequest.md) objects.|
|[Get offerShiftRequest](../api/offershiftrequest-get.md)|[offerShiftRequest](../resources/offershiftrequest.md)|Read properties and relationships of the [offerShiftRequest](../resources/offershiftrequest.md) object.|
|[Create offerShiftRequest](../api/offershiftrequest-create.md)|[offerShiftRequest](../resources/offershiftrequest.md)|Create a new [offerShiftRequest](../resources/offershiftrequest.md) object.|
|[Delete offerShiftRequest](../api/offershiftrequest-delete.md)|None|Deletes a [offerShiftRequest](../resources/offershiftrequest.md).|
|[Update offerShiftRequest](../api/offershiftrequest-update.md)|[offerShiftRequest](../resources/offershiftrequest.md)|Update the properties of a [offerShiftRequest](../resources/offershiftrequest.md) object.|
|[approve](../api/offershiftrequest-approve.md)|None||
|[decline](../api/offershiftrequest-decline.md)|None||
|[List offerShiftRequests](../api/schedule-list-offershiftrequests.md)|[offerShiftRequest](../resources/offershiftrequest.md) collection|Get the offerShiftRequests from the offerShiftRequests navigation property.|
|[Add offerShiftRequests](../api/schedule-post-offershiftrequests.md)|[offerShiftRequest](../resources/offershiftrequest.md)|Add offerShiftRequests by posting to the offerShiftRequests collection.|

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
|recipientActionDateTime|DateTimeOffset||
|recipientActionMessage|String||
|recipientUserId|String||
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderShiftId|String||
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

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

