---
title: "invitationParticipantInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# invitationParticipantInfo resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|endpointType|Enumeration|. Possible values are: `default`, `voicemail`, `skypeForBusiness`, `skypeForBusinessVoipPhone`, `unknownFutureValue`.|
|identity|[identitySet](../resources/identityset.md)||
|replacesCallId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.invitationParticipantInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.invitationParticipantInfo",
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
  "endpointType": "String",
  "replacesCallId": "String"
}
```

