---
title: "onlineMeeting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# onlineMeeting resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onlineMeeting](../api/onlinemeeting-get.md)|[onlineMeeting](../resources/onlinemeeting.md)|Read properties and relationships of the [onlineMeeting](../resources/onlinemeeting.md) object.|
|[Update onlineMeeting](../api/onlinemeeting-update.md)|[onlineMeeting](../resources/onlinemeeting.md)|Update the properties of a [onlineMeeting](../resources/onlinemeeting.md) object.|
|[List onlineMeetings](../api/user-list-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md) collection|Get the onlineMeetings from the onlineMeetings navigation property.|
|[Add onlineMeetings](../api/user-post-onlinemeetings.md)|[onlineMeeting](../resources/onlinemeeting.md)|Add onlineMeetings by posting to the onlineMeetings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessLevel|Enumeration|. Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `sameEnterpriseAndFederated`.|
|audioConferencing|[audioConferencing](../resources/audioconferencing.md)||
|canceledDateTime|DateTimeOffset||
|capabilities|Enumeration collection||
|chatInfo|[chatInfo](../resources/chatinfo.md)||
|creationDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|entryExitAnnouncement|Boolean||
|expirationDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|isBroadcast|Boolean||
|isCancelled|Boolean||
|joinUrl|String||
|participants|[meetingParticipants](../resources/meetingparticipants.md)||
|startDateTime|DateTimeOffset||
|subject|String||
|videoTeleconferenceId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onlineMeeting",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onlineMeeting",
  "id": "String (identifier)",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "canceledDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)",
  "entryExitAnnouncement": true,
  "joinUrl": "String",
  "subject": "String",
  "isCancelled": true,
  "participants": {
    "@odata.type": "microsoft.graph.meetingParticipants"
  },
  "isBroadcast": true,
  "accessLevel": "String",
  "capabilities": [
    "String"
  ],
  "audioConferencing": {
    "@odata.type": "microsoft.graph.audioConferencing"
  },
  "chatInfo": {
    "@odata.type": "microsoft.graph.chatInfo"
  },
  "videoTeleconferenceId": "String"
}
```

