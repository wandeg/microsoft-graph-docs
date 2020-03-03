---
title: "contentInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# contentInfo resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|format|Enumeration|. Possible values are: `default`, `email`.|
|identifier|String||
|metadata|[keyValuePair](../resources/keyValuePair.md) collection||
|state|Enumeration|. Possible values are: `rest`, `motion`, `use`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.contentInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.contentInfo",
  "format": "String",
  "state": "String",
  "identifier": "String",
  "metadata": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```

