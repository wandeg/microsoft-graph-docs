---
title: "onlineMeeting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# onlineMeeting resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get onlineMeeting](../api/onlinemeeting-get.md)|[onlineMeeting](../resources/onlinemeeting.md)|Read the properties and relationships of an [onlineMeeting](../resources/onlinemeeting.md) object.|
|[Update onlineMeeting](../api/onlinemeeting-update.md)|[onlineMeeting](../resources/onlinemeeting.md)|Update the properties of an [onlineMeeting](../resources/onlinemeeting.md) object.|
|[createOrGet](../api/onlinemeeting-createorget.md)|[onlineMeeting](../resources/onlinemeeting.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accessLevel|accessLevel|**TODO: Add Description**. Possible values are: `everyone`, `invited`, `locked`, `sameEnterprise`, `sameEnterpriseAndFederated`.|
|audioConferencing|[audioConferencing](../resources/audioconferencing.md)|**TODO: Add Description**|
|canceledDateTime|DateTimeOffset|**TODO: Add Description**|
|capabilities|meetingCapabilities collection|**TODO: Add Description**|
|chatInfo|[chatInfo](../resources/chatinfo.md)|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|entryExitAnnouncement|Boolean|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isBroadcast|Boolean|**TODO: Add Description**|
|isCancelled|Boolean|**TODO: Add Description**|
|joinInformation|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|joinUrl|String|**TODO: Add Description**|
|participants|[meetingParticipants](../resources/meetingparticipants.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|videoTeleconferenceId|String|**TODO: Add Description**|

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
  "videoTeleconferenceId": "String",
  "externalId": "String",
  "joinInformation": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```

