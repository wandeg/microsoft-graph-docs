---
title: "sharingInvitation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# sharingInvitation resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|email|String||
|invitedBy|[identitySet](../resources/identitySet.md)||
|redeemedBy|String||
|signInRequired|Boolean||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharingInvitation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharingInvitation",
  "email": "String",
  "invitedBy": {
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
  "redeemedBy": "String",
  "signInRequired": true
}
```

