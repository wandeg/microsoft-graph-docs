---
title: "meetingParticipants resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# meetingParticipants resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|attendees|[meetingParticipantInfo](../resources/meetingparticipantinfo.md) collection|**TODO: Add Description**|
|organizer|[meetingParticipantInfo](../resources/meetingparticipantinfo.md)|**TODO: Add Description**|

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
    "upn": "String"
  },
  "attendees": [
    {
      "@odata.type": "microsoft.graph.meetingParticipantInfo"
    }
  ]
}
```

