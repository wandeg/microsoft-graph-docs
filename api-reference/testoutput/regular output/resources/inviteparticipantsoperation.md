---
title: "inviteParticipantsOperation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# inviteParticipantsOperation resource type


Namespace: microsoft.graph




Inherits from [commsOperation](../resources/commsoperation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List inviteParticipantsOperations](../api/inviteparticipantsoperation-list.md)|[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) collection|List properties and relationships of the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) objects.|
|[Get inviteParticipantsOperation](../api/inviteparticipantsoperation-get.md)|[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)|Read properties and relationships of the [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object.|
|[Create inviteParticipantsOperation](../api/inviteparticipantsoperation-create.md)|[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)|Create a new [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object.|
|[Delete inviteParticipantsOperation](../api/inviteparticipantsoperation-delete.md)|None|Deletes a [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md).|
|[Update inviteParticipantsOperation](../api/inviteparticipantsoperation-update.md)|[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)|Update the properties of a [inviteParticipantsOperation](../resources/inviteparticipantsoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientContext|String| Inherited from [commsOperation](../resources/commsoperation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|participants|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection||
|resultInfo|[resultInfo](../resources/resultinfo.md)| Inherited from [commsOperation](../resources/commsoperation.md)|
|status|Enumeration| Inherited from [commsOperation](../resources/commsoperation.md). Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.inviteParticipantsOperation",
  "baseType": "microsoft.graph.commsOperation",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.inviteParticipantsOperation",
  "id": "String (identifier)",
  "status": "String",
  "clientContext": "String",
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "participants": [
    {
      "@odata.type": "microsoft.graph.invitationParticipantInfo"
    }
  ]
}
```

