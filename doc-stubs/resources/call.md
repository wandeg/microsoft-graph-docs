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


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[logTeleconferenceDeviceQuality](../api/call-logteleconferencedevicequality.md)|None|**TODO: Add Description**|
|[answer](../api/call-answer.md)|None|**TODO: Add Description**|
|[changeScreenSharingRole](../api/call-changescreensharingrole.md)|None|**TODO: Add Description**|
|[keepAlive](../api/call-keepalive.md)|None|**TODO: Add Description**|
|[mute](../api/call-mute.md)|[muteParticipantOperation](../resources/muteparticipantoperation.md)|**TODO: Add Description**|
|[playPrompt](../api/call-playprompt.md)|[playPromptOperation](../resources/playpromptoperation.md)|**TODO: Add Description**|
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
|[Get participants](../api/call-get-participant.md)|[participant](../resources/participant.md)|Read the properties and relationships of a [participant](../resources/participant.md) object.|
|[List operations](../api/call-list-operations.md)|[commsOperation](../resources/commsoperation.md) collection|Get the commsOperations from the operations navigation property.|
|[Create operations](../api/call-post-operations.md)|[commsOperation](../resources/commsoperation.md)|Create a new operations object.|
|[Delete operations](../api/call-delete-operations.md)|None|Delete a [commsOperation](../resources/commsoperation.md) object.|
|[Update operations](../api/call-update-operations.md)|[commsOperation](../resources/commsoperation.md)|Update the properties of an operations object.|
|[Get operations](../api/call-get-commsoperation.md)|[commsOperation](../resources/commsoperation.md)|Read the properties and relationships of a [commsOperation](../resources/commsoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
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
|meetingInfo|[meetingInfo](../resources/meetinginfo.md)|**TODO: Add Description**|
|myParticipantId|String|**TODO: Add Description**|
|requestedModalities|modality collection|**TODO: Add Description**|
|resultInfo|[resultInfo](../resources/resultinfo.md)|**TODO: Add Description**|
|source|[participantInfo](../resources/participantinfo.md)|**TODO: Add Description**|
|state|callState|**TODO: Add Description**. Possible values are: `incoming`, `establishing`, `established`, `hold`, `transferring`, `transferAccepted`, `redirecting`, `terminating`, `terminated`, `unknownFutureValue`.|
|subject|String|**TODO: Add Description**|
|targets|[invitationParticipantInfo](../resources/invitationparticipantinfo.md) collection|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|toneInfo|[toneInfo](../resources/toneinfo.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|operations|[commsOperation](../resources/commsoperation.md) collection|**TODO: Add Description**|
|participants|[participant](../resources/participant.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.callMediaState"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "direction": "String",
  "subject": "String",
  "callbackUri": "String",
  "callRoutes": [
    {
      "@odata.type": "microsoft.graph.callRoute"
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
  "requestedModalities": [
    "String"
  ],
  "mediaConfig": {
    "@odata.type": "microsoft.graph.mediaConfig"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "callOptions": {
    "@odata.type": "microsoft.graph.callOptions"
  },
  "meetingInfo": {
    "@odata.type": "microsoft.graph.meetingInfo"
  },
  "tenantId": "String",
  "myParticipantId": "String",
  "toneInfo": {
    "@odata.type": "microsoft.graph.toneInfo"
  },
  "callChainId": "String",
  "incomingContext": {
    "@odata.type": "microsoft.graph.incomingContext"
  }
}
```

