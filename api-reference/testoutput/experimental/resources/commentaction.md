---
title: "commentAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# commentAction resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|isReply|Boolean||
|parentAuthor|[identitySet](../resources/identityset.md)||
|participants|[identitySet](../resources/identityset.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.commentAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.commentAction",
  "isReply": true,
  "parentAuthor": {
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
  "participants": [
    {
      "@odata.type": "microsoft.graph.identitySet"
    }
  ]
}
```

