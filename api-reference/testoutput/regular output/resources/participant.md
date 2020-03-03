---
title: "participant resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# participant resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get participant](../api/participant-get.md)|[participant](../resources/participant.md)|Read properties and relationships of the [participant](../resources/participant.md) object.|
|[Delete participant](../api/participant-delete.md)|None|Deletes a [participant](../resources/participant.md).|
|[Update participant](../api/participant-update.md)|[participant](../resources/participant.md)|Update the properties of a [participant](../resources/participant.md) object.|
|[invite](../api/participant-invite.md)|[inviteParticipantsOperation](../resources/inviteParticipantsOperation.md)||
|[mute](../api/participant-mute.md)|[muteParticipantOperation](../resources/muteParticipantOperation.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantInfo.md)||
|isInLobby|Boolean||
|isMuted|Boolean||
|mediaStreams|[mediaStream](../resources/mediaStream.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.participant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.participant",
  "id": "String (identifier)",
  "info": {
    "@odata.type": "microsoft.graph.participantInfo"
  },
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream"
    }
  ],
  "isMuted": true,
  "isInLobby": true
}
```

