---
title: "call resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# call resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get call](../api/call-get.md)|[call](../resources/call.md)|Read properties and relationships of the [call](../resources/call.md) object.|
|[Delete call](../api/call-delete.md)|None|Deletes a [call](../resources/call.md).|
|[Update call](../api/call-update.md)|[call](../resources/call.md)|Update the properties of a [call](../resources/call.md) object.|
|[answer](../api/call-answer.md)|None||
|[changeScreenSharingRole](../api/call-changescreensharingrole.md)|None||
|[mute](../api/call-mute.md)|[muteParticipantOperation](../resources/muteParticipantOperation.md)||
|[playPrompt](../api/call-playprompt.md)|[playPromptOperation](../resources/playPromptOperation.md)||
|[record](../api/call-record.md)|[recordOperation](../resources/recordOperation.md)||
|[redirect](../api/call-redirect.md)|None||
|[reject](../api/call-reject.md)|None||
|[subscribeToTone](../api/call-subscribetotone.md)|[subscribeToToneOperation](../resources/subscribeToToneOperation.md)||
|[transfer](../api/call-transfer.md)|None||
|[unmute](../api/call-unmute.md)|[unmuteParticipantOperation](../resources/unmuteParticipantOperation.md)||
|[List participants](../api/call-list-participants.md)|[participant](../resources/participant.md) collection|Get the participants from the participants navigation property.|
|[Add participants](../api/call-post-participants.md)|[participant](../resources/participant.md)|Add participants by posting to the participants collection.|
|[List operations](../api/call-list-operations.md)|[commsOperation](../resources/commsOperation.md) collection|Get the commsOperations from the operations navigation property.|
|[Add operations](../api/call-post-operations.md)|[commsOperation](../resources/commsOperation.md)|Add operations by posting to the operations collection.|
|[List calls](../api/cloudcommunications-list-calls.md)|[call](../resources/call.md) collection|Get the calls from the calls navigation property.|
|[Add calls](../api/cloudcommunications-post-calls.md)|[call](../resources/call.md)|Add calls by posting to the calls collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|callbackUri|String||
|chatInfo|[chatInfo](../resources/chatInfo.md)||
|direction|Enumeration|. Possible values are: `incoming`, `outgoing`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|mediaConfig|[mediaConfig](../resources/mediaConfig.md)||
|mediaState|[callMediaState](../resources/callMediaState.md)||
|meetingInfo|[meetingInfo](../resources/meetingInfo.md)||
|myParticipantId|String||
|requestedModalities|Enumeration collection||
|resultInfo|[resultInfo](../resources/resultInfo.md)||
|source|[participantInfo](../resources/participantInfo.md)||
|state|Enumeration|. Possible values are: `incoming`, `establishing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|subject|String||
|targets|[participantInfo](../resources/participantInfo.md) collection||
|tenantId|String||
|toneInfo|[toneInfo](../resources/toneInfo.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|operations|[commsOperation](../resources/commsOperation.md) collection||
|participants|[participant](../resources/participant.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.call",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.call",
  "id": "String (identifier)",
  "state": "String",
  "mediaState": {
    "@odata.type": "microsoft.graph.callMediaState",
    "audio": "String"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "direction": "String",
  "subject": "String",
  "callbackUri": "String",
  "source": {
    "@odata.type": "microsoft.graph.participantInfo",
    "identity": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "displayName": "String",
        "id": "String"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "region": "String",
    "languageId": "String"
  },
  "targets": [
    {
      "@odata.type": "microsoft.graph.participantInfo"
    }
  ],
  "requestedModalities": [
    "String"
  ],
  "mediaConfig": {
    "@odata.type": "microsoft.graph.mediaConfig"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo",
    "threadId": "String",
    "messageId": "String",
    "replyChainMessageId": "String"
  },
  "meetingInfo": {
    "@odata.type": "microsoft.graph.meetingInfo"
  },
  "tenantId": "String",
  "myParticipantId": "String",
  "toneInfo": {
    "@odata.type": "microsoft.graph.toneInfo",
    "sequenceId": 1024,
    "tone": "String"
  }
}
```

