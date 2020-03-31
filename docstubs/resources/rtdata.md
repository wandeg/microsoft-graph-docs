---
title: "RTData resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# RTData resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|attribute|[RTAttribute](../resources/rtattribute.md) collection||
|endIdx|Int32||
|startIdx|Int32||
|type|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.RTData"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.RTData",
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
```

