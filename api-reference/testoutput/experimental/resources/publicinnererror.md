---
title: "publicInnerError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# publicInnerError resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|details|[publicErrorDetail](../resources/publicErrorDetail.md) collection||
|message|String||
|target|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicInnerError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicInnerError",
  "code": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.publicErrorDetail",
      "message": "String",
      "target": "String"
    }
  ],
  "message": "String",
  "target": "String"
}
```

