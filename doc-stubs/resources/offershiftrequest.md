---
title: "offerShiftRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# offerShiftRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [scheduleChangeRequest](../resources/schedulechangerequest.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[approve](../api/offershiftrequest-approve.md)|None|**TODO: Add Description**|
|[decline](../api/offershiftrequest-decline.md)|None|**TODO: Add Description**|
|[List offerShiftRequests](../api/schedule-list-offershiftrequests.md)|[offerShiftRequest](../resources/offershiftrequest.md) collection|Get the offerShiftRequests from the offerShiftRequests navigation property.|
|[Create offerShiftRequests](../api/schedule-post-offershiftrequests.md)|[offerShiftRequest](../resources/offershiftrequest.md)|Create a new offerShiftRequests object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedTo|scheduleChangeRequestActor|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `sender`, `recipient`, `manager`, `system`, `unknownFutureValue`.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|managerActionDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerActionMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|managerUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|recipientActionDateTime|DateTimeOffset|**TODO: Add Description**|
|recipientActionMessage|String|**TODO: Add Description**|
|recipientUserId|String|**TODO: Add Description**|
|senderDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderMessage|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|senderShiftId|String|**TODO: Add Description**|
|senderUserId|String|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md)|
|state|scheduleChangeState|**TODO: Add Description** Inherited from [scheduleChangeRequest](../resources/schedulechangerequest.md). Possible values are: `pending`, `approved`, `declined`, `unknownFutureValue`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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

