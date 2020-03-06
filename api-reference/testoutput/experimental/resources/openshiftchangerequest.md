---
title: "openShiftChangeRequest resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# openShiftChangeRequest resource type


Namespace: microsoft.graph




Inherits from [scheduleChangeRequest](../resources/schedulechangerequest.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get openShiftChangeRequest](../api/openshiftchangerequest-get.md)|[openShiftChangeRequest](../resources/openshiftchangerequest.md)|Read properties and relationships of the [openShiftChangeRequest](../resources/openshiftchangerequest.md) object.|
|[approve](../api/openshiftchangerequest-approve.md)|None||
|[decline](../api/openshiftchangerequest-decline.md)|None||
|[List openShiftChangeRequests](../api/schedule-list-openshiftchangerequests.md)|[openShiftChangeRequest](../resources/openshiftchangerequest.md) collection|Get the openShiftChangeRequests from the openShiftChangeRequests navigation property.|
|[Add openShiftChangeRequests](../api/schedule-post-openshiftchangerequests.md)|[openShiftChangeRequest](../resources/openshiftchangerequest.md)|Add openShiftChangeRequests by posting to the openShiftChangeRequests collection.|

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
|openShiftId|String||
|senderDateTime|DateTimeOffset| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderUserId|String| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|state|Enumeration| Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.openShiftChangeRequest",
  "baseType": "microsoft.graph.scheduleChangeRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.openShiftChangeRequest",
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
  "openShiftId": "String"
}
```

