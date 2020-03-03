---
title: "callRoute resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# callRoute resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|final|[identitySet](../resources/identityset.md)||
|original|[identitySet](../resources/identityset.md)||
|routingType|Enumeration|. Possible values are: `forwarded`, `lookup`, `selfFork`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRoute",
  "routingType": "String",
  "original": {
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
  "final": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

