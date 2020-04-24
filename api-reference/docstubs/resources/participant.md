---
title: "participant resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# participant resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get participant](../api/participant-get.md)|[participant](../resources/participant.md)|Read the properties and relationships of a [participant](../resources/participant.md) object.|
|[Update participant](../api/participant-update.md)|[participant](../resources/participant.md)|Update the properties of a [participant](../resources/participant.md) object.|
|[invite](../api/participant-invite.md)|[inviteParticipantsOperation](../resources/inviteparticipantsoperation.md)|**TODO: Add Description**|
|[muteAll](../api/participant-muteall.md)|[muteParticipantsOperation](../resources/muteparticipantsoperation.md)|**TODO: Add Description**|
|[mute](../api/participant-mute.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|info|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|isInLobby|Boolean|**TODO: Add Description**|
|isMuted|Boolean|**TODO: Add Description**|
|mediaStreams|[mediaStream](../resources/mediastream.md) collection|**TODO: Add Description**|
|metadata|String|**TODO: Add Description**|
|recordingInfo|[recordingInfo](../resources/recordinginfo.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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
  "recordingInfo": {
    "@odata.type": "microsoft.graph.recordingInfo"
  },
  "mediaStreams": [
    {
      "@odata.type": "microsoft.graph.mediaStream"
    }
  ],
  "metadata": "String",
  "isMuted": true,
  "isInLobby": true
}
```

