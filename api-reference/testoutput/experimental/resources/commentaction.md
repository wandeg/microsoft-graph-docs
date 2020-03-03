---
title: "commentAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# commentAction resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|isReply|Boolean||
|parentAuthor|[identitySet](../resources/identitySet.md)||
|participants|[identitySet](../resources/identitySet.md) collection||

## Relationships
None

## JSON Representation
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

