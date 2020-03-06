---
title: "educationFeedback resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationFeedback resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedbackBy|[identitySet](../resources/identityset.md)||
|feedbackDateTime|DateTimeOffset||
|text|[educationItemBody](../resources/educationitembody.md)||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationFeedback"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationFeedback",
  "text": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "String"
  },
  "feedbackDateTime": "String (timestamp)",
  "feedbackBy": {
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

