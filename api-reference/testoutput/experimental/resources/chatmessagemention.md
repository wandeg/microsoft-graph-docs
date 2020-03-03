---
title: "chatMessageMention resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# chatMessageMention resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|Int32||
|mentioned|[identitySet](../resources/identitySet.md)||
|mentionText|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.chatMessageMention",
  "id": "String (identifier)",
  "mentionText": "String",
  "mentioned": {
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

