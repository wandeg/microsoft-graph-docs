---
title: "call resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# call resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get call](../api/call-get.md)|[call](../resources/call.md)|Read properties and relationships of the [call](../resources/call.md) object.|
|[Update call](../api/call-update.md)|[call](../resources/call.md)|Update the properties of a [call](../resources/call.md) object.|
|[logTeleconferenceDeviceQuality](../api/call-logteleconferencedevicequality.md)|None||
|[answer](../api/call-answer.md)|None||
|[cancelMediaProcessing](../api/call-cancelmediaprocessing.md)|[cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md)||
|[changeScreenSharingRole](../api/call-changescreensharingrole.md)|None||
|[keepAlive](../api/call-keepalive.md)|None||
|[mute](../api/call-mute.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)||
|[playPrompt](../api/call-playprompt.md)|[playPromptOperation](../resources/playpromptoperation.md)||
|[record](../api/call-record.md)|[recordOperation](../resources/recordoperation.md)||
|[recordResponse](../api/call-recordresponse.md)|[recordOperation](../resources/recordoperation.md)||
|[redirect](../api/call-redirect.md)|None||
|[reject](../api/call-reject.md)|None||
|[subscribeToTone](../api/call-subscribetotone.md)|[subscribeToToneOperation](../resources/subscribetotoneoperation.md)||
|[transfer](../api/call-transfer.md)|None||
|[unmute](../api/call-unmute.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md)||
|[updateRecordingStatus](../api/call-updaterecordingstatus.md)|[updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md)||
|[List participants](../api/call-list-participants.md)|[participant](../resources/participant.md) collection|Get the participants from the participants navigation property.|
|[Add participants](../api/call-post-participants.md)|[participant](../resources/participant.md)|Add participants by posting to the participants collection.|
|[List audioRoutingGroups](../api/call-list-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md) collection|Get the audioRoutingGroups from the audioRoutingGroups navigation property.|
|[Add audioRoutingGroups](../api/call-post-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Add audioRoutingGroups by posting to the audioRoutingGroups collection.|
|[List operations](../api/call-list-operations.md)|[commsOperation](../resources/commsoperation.md) collection|Get the commsOperations from the operations navigation property.|
|[Add operations](../api/call-post-operations.md)|[commsOperation](../resources/commsoperation.md)|Add operations by posting to the operations collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeModalities|Enumeration collection||
|answeredBy|[participantInfo](../resources/participantinfo.md)||
|callbackUri|String||
|callChainId|String||
|callOptions|[callOptions](../resources/calloptions.md)||
|callRoutes|[callRoute](../resources/callroute.md) collection||
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|direction|Enumeration| Possible values are: `incoming`, `outgoing`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|incomingContext|[incomingContext](../resources/incomingcontext.md)||
|mediaConfig|[mediaConfig](../resources/mediaconfig.md)||
|mediaState|[callMediaState](../resources/callmediastate.md)||
|meetingCapability|[meetingCapability](../resources/meetingcapability.md)||
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)||
|myParticipantId|String||
|requestedModalities|Enumeration collection||
|resultInfo|[ResultInfo](../resources/resultinfo.md)||
|ringingTimeoutInSeconds|Int32||
|routingPolicies|Enumeration collection||
|source|[participantInfo](../resources/participantinfo.md)||
|state|Enumeration| Possible values are: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|subject|String||
|targets|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection||
|tenantId|String||
|terminationReason|String||
|toneInfo|[toneInfo](../resources/toneinfo.md)||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|audioRoutingGroups|[audioRoutingGroup](../resources/audioroutinggroup.md) collection||
|operations|[commsOperation](../resources/commsoperation.md) collection||
|participants|[participant](../resources/participant.md) collection||

## JSON representation
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
    "@odata.type": "microsoft.graph.ResultInfo"
  },
  "terminationReason": "String",
  "direction": "String",
  "ringingTimeoutInSeconds": 1024,
  "subject": "String",
  "callbackUri": "String",
  "callRoutes": [
    {
      "@odata.type": "microsoft.graph.callRoute",
      "routingType": "String",
      "original": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "final": {
        "@odata.type": "microsoft.graph.identitySet"
      }
    }
  ],
  "source": {
    "@odata.type": "microsoft.graph.participantInfo"
  },
  "targets": [
    {
      "@odata.type": "microsoft.graph.invitationParticipantInfo"
    }
  ],
  "answeredBy": {
    "@odata.type": "microsoft.graph.participantInfo"
  },
  "requestedModalities": [
    "String"
  ],
  "activeModalities": [
    "String"
  ],
  "mediaConfig": {
    "@odata.type": "microsoft.graph.mediaConfig",
    "removeFromDefaultAudioGroup": true
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo",
    "threadId": "String",
    "messageId": "String",
    "replyChainMessageId": "String"
  },
  "callOptions": {
    "@odata.type": "microsoft.graph.callOptions"
  },
  "meetingInfo": {
    "@odata.type": "microsoft.graph.meetingInfo",
    "allowConversationWithoutHost": true
  },
  "meetingCapability": {
    "@odata.type": "microsoft.graph.meetingCapability",
    "allowAnonymousUsersToDialOut": true,
    "autoAdmittedUsers": "String",
    "allowAnonymousUsersToStartMeeting": true
  },
  "routingPolicies": [
    "String"
  ],
  "tenantId": "String",
  "myParticipantId": "String",
  "toneInfo": {
    "@odata.type": "microsoft.graph.toneInfo",
    "sequenceId": 1024,
    "tone": "String"
  },
  "callChainId": "String",
  "incomingContext": {
    "@odata.type": "microsoft.graph.incomingContext",
    "sourceParticipantId": "String",
    "observedParticipantId": "String",
    "onBehalfOf": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "transferor": {
      "@odata.type": "microsoft.graph.identitySet"
    }
  }
}
```

