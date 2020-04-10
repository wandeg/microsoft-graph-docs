---
title: "publicError resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# publicError resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|code|String||
|details|[publicErrorDetail](../resources/publicerrordetail.md) collection||
|innerError|[publicInnerError](../resources/publicinnererror.md)||
|message|String||
|target|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.publicError"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.publicError",
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
```

