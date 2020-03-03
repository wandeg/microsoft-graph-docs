---
title: "organizerMeetingInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# organizerMeetingInfo resource type


Namespace: microsoft.graph




Inherits from [meetingInfo](../resources/meetinginfo.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowConversationWithoutHost|Boolean| Inherited from [meetingInfo](../resources/meetinginfo.md)|
|organizer|[identitySet](../resources/identityset.md)||

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

