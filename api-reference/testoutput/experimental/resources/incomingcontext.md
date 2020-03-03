---
title: "incomingContext resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# incomingContext resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|observedParticipantId|String||
|onBehalfOf|[identitySet](../resources/identitySet.md)||
|sourceParticipantId|String||
|transferor|[identitySet](../resources/identitySet.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.incomingContext"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incomingContext",
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {
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
  "transferor": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

