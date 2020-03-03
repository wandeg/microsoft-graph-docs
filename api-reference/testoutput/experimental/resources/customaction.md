---
title: "customAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# customAction resource type




Inherits from [informationProtectionAction](../resources/informationProtectionAction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|String||
|properties|[keyValuePair](../resources/keyValuePair.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customAction",
  "name": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "value": "String"
    }
  ]
}
```

