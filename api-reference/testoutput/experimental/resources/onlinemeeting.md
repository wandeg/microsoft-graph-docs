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
|[List onlineMeetings](../api/onlinemeeting-list.md)|[onlineMeeting](../resources/onlinemeeting.md) collection|List properties and relationships of the [onlineMeeting](../resources/onlinemeeting.md) objects.|
|[Get onlineMeeting](../api/onlinemeeting-get.md)|[onlineMeeting](../resources/onlinemeeting.md)|Read properties and relationships of the [onlineMeeting](../resources/onlinemeeting.md) object.|
|[Create onlineMeeting](../api/onlinemeeting-create.md)|[onlineMeeting](../resources/onlinemeeting.md)|Create a new [onlineMeeting](../resources/onlinemeeting.md) object.|
|[Delete onlineMeeting](../api/onlinemeeting-delete.md)|None|Deletes a [onlineMeeting](../resources/onlinemeeting.md).|
|[Update onlineMeeting](../api/onlinemeeting-update.md)|[onlineMeeting](../resources/onlinemeeting.md)|Update the properties of a [onlineMeeting](../resources/onlinemeeting.md) object.|

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

## JSON Representation
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

