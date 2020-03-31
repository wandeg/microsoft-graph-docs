---
title: "publicInnerError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# publicInnerError resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|details|[publicErrorDetail](../resources/publicerrordetail.md) collection||
|message|String||
|target|String||

## Relationships
None

## JSON representation
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

