---
title: "organizerMeetingInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# organizerMeetingInfo resource type




Inherits from [meetingInfo](../resources/meetingInfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowConversationWithoutHost|Boolean| Inherited from [meetingInfo](../resources/meetingInfo.md)|
|organizer|[identitySet](../resources/identitySet.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.organizerMeetingInfo",
  "allowConversationWithoutHost": true,
  "organizer": {
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
  }
}
```

