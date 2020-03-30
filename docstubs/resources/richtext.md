---
title: "RichText resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# RichText resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|rawText|String||
|rtData|[RTData](../resources/rtdata.md) collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.RichText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.RichText",
  "rawText": "String",
  "rtData": [
    {
      "@odata.type": "microsoft.graph.RTData",
      "type": "String",
      "startIdx": 1024,
      "endIdx": 1024,
      "attribute": [
        {
          "@odata.type": "microsoft.graph.RTAttribute",
          "name": "String",
          "value": "String"
        }
      ]
    }
  ]
}
```

