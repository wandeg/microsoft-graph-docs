---
title: "publicErrorResponse resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# publicErrorResponse resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|error|[publicError](../resources/publicError.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicErrorResponse"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicErrorResponse",
  "error": {
    "@odata.type": "microsoft.graph.publicError",
    "code": "String",
    "message": "String",
    "target": "String",
    "details": [
      {
        "@odata.type": "microsoft.graph.publicErrorDetail"
      }
    ],
    "innerError": {
      "@odata.type": "microsoft.graph.publicInnerError"
    }
  }
}
```

