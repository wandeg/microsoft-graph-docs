---
title: "meetingParticipants resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# meetingParticipants resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendees|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection||
|contributors|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection||
|organizer|[meetingParticipantInfo](../resources/meetingparticipantinfo.md)||
|producers|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingParticipants"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.meetingParticipants",
  "organizer": {
    "@odata.type": "microsoft.graph.meetingParticipantInfo",
    "identity": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "String",
        "displayName": "String"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "upn": "String"
  },
  "attendees": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ],
  "producers": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ],
  "contributors": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ]
}
```

