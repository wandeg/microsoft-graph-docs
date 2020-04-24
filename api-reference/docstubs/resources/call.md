---
title: "call resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# call resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get call](../api/call-get.md)|[call](../resources/call.md)|Read the properties and relationships of a [call](../resources/call.md) object.|
|[Update call](../api/call-update.md)|[call](../resources/call.md)|Update the properties of a [call](../resources/call.md) object.|
|[logTeleconferenceDeviceQuality](../api/call-logteleconferencedevicequality.md)|None|**TODO: Add Description**|
|[answer](../api/call-answer.md)|None|**TODO: Add Description**|
|[cancelMediaProcessing](../api/call-cancelmediaprocessing.md)|[cancelMediaProcessingOperation](../resources/cancelmediaprocessingoperation.md)|**TODO: Add Description**|
|[changeScreenSharingRole](../api/call-changescreensharingrole.md)|None|**TODO: Add Description**|
|[keepAlive](../api/call-keepalive.md)|None|**TODO: Add Description**|
|[mute](../api/call-mute.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)|**TODO: Add Description**|
|[playPrompt](../api/call-playprompt.md)|[playPromptOperation](../resources/playpromptoperation.md)|**TODO: Add Description**|
|[record](../api/call-record.md)|[recordOperation](../resources/recordoperation.md)|**TODO: Add Description**|
|[recordResponse](../api/call-recordresponse.md)|[recordOperation](../resources/recordoperation.md)|**TODO: Add Description**|
|[redirect](../api/call-redirect.md)|None|**TODO: Add Description**|
|[reject](../api/call-reject.md)|None|**TODO: Add Description**|
|[subscribeToTone](../api/call-subscribetotone.md)|[subscribeToToneOperation](../resources/subscribetotoneoperation.md)|**TODO: Add Description**|
|[transfer](../api/call-transfer.md)|None|**TODO: Add Description**|
|[unmute](../api/call-unmute.md)|[unmuteParticipantOperation](../resources/unmuteparticipantoperation.md)|**TODO: Add Description**|
|[updateRecordingStatus](../api/call-updaterecordingstatus.md)|[updateRecordingStatusOperation](../resources/updaterecordingstatusoperation.md)|**TODO: Add Description**|
|[List participants](../api/call-list-participants.md)|[participant](../resources/participant.md) collection|Get the participants from the participants navigation property.|
|[Create participants](../api/call-post-participants.md)|[participant](../resources/participant.md)|Create a new participants object.|
|[Delete participants](../api/call-delete-participants.md)|None|Delete a [participant](../resources/participant.md) object.|
|[Update participants](../api/call-update-participants.md)|[participant](../resources/participant.md)|Update the properties of a participants object.|
|[Get participant](../api/participant-get.md)|[participant](../resources/participant.md)|Read the properties and relationships of a [participant](../resources/participant.md) object.|
|[List audioRoutingGroups](../api/call-list-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md) collection|Get the audioRoutingGroups from the audioRoutingGroups navigation property.|
|[Create audioRoutingGroups](../api/call-post-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Create a new audioRoutingGroups object.|
|[Delete audioRoutingGroups](../api/call-delete-audioroutinggroups.md)|None|Delete an [audioRoutingGroup](../resources/audioroutinggroup.md) object.|
|[Update audioRoutingGroups](../api/call-update-audioroutinggroups.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Update the properties of an audioRoutingGroups object.|
|[Get audioRoutingGroup](../api/audioroutinggroup-get.md)|[audioRoutingGroup](../resources/audioroutinggroup.md)|Read the properties and relationships of an [audioRoutingGroup](../resources/audioroutinggroup.md) object.|
|[List operations](../api/call-list-operations.md)|[commsOperation](../resources/commsoperation.md) collection|Get the commsOperations from the operations navigation property.|
|[Create operations](../api/call-post-operations.md)|[commsOperation](../resources/commsoperation.md)|Create a new operations object.|
|[Delete operations](../api/call-delete-operations.md)|None|Delete an [commsOperation](../resources/commsoperation.md) object.|
|[Update operations](../api/call-update-operations.md)|[commsOperation](../resources/commsoperation.md)|Update the properties of an operations object.|
|[Get commsOperation](../api/commsoperation-get.md)|[commsOperation](../resources/commsoperation.md)|Read the properties and relationships of a [commsOperation](../resources/commsoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activeModalities|modality collection|**TODO: Add Description**|
|answeredBy|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|callbackUri|String|**TODO: Add Description**|
|callChainId|String|**TODO: Add Description**|
|callOptions|[callOptions](../resources/calloptions.md)|**TODO: Add Description**|
|callRoutes|[callRoute](../resources/callroute.md) collection|**TODO: Add Description**|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|direction|callDirection|**TODO: Add Description**. Possible values are: `incoming`, `outgoing`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|incomingContext|[incomingContext](../resources/incomingcontext.md)|**TODO: Add Description**|
|mediaConfig|[mediaConfig](../resources/mediaconfig.md)|**TODO: Add Description**|
|mediaState|[callMediaState](../resources/callmediastate.md)|**TODO: Add Description**|
|meetingCapability|[meetingCapability](../resources/meetingcapability.md)|**TODO: Add Description**|
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)|**TODO: Add Description**|
|myParticipantId|String|**TODO: Add Description**|
|requestedModalities|modality collection|**TODO: Add Description**|
|resultInfo|[ResultInfo](../resources/resultinfo.md)|**TODO: Add Description**|
|ringingTimeoutInSeconds|Int32|**TODO: Add Description**|
|routingPolicies|routingPolicy collection|**TODO: Add Description**|
|source|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|state|callState|**TODO: Add Description**. Possible values are: `incoming`, `establishing`, `ringing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|subject|String|**TODO: Add Description**|
|targets|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|terminationReason|String|**TODO: Add Description**|
|toneInfo|[toneInfo](../resources/toneinfo.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|audioRoutingGroups|[audioRoutingGroup](../resources/audioroutinggroup.md) collection|**TODO: Add Description**|
|operations|[commsOperation](../resources/commsoperation.md) collection|**TODO: Add Description**|
|participants|[participant](../resources/participant.md) collection|**TODO: Add Description**|

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

