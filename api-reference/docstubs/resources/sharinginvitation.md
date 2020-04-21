---
title: "sharingInvitation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# sharingInvitation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|email|String|**TODO: Add Description**|
|invitedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|redeemedBy|String|**TODO: Add Description**|
|signInRequired|Boolean|**TODO: Add Description**|

## Relationships
None

## JSON representation
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
  "redeemedBy": "String",
  "signInRequired": true
}
```

