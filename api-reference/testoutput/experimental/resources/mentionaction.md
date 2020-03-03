---
title: "mentionAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# mentionAction resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|mentionees|[identitySet](../resources/identitySet.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mentionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mentionAction",
  "mentionees": [
    {
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
  ]
}
```

