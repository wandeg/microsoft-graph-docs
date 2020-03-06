---
title: "customAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# customAction resource type


Namespace: microsoft.graph




Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|name|String||
|properties|[keyValuePair](../resources/keyvaluepair.md) collection||

## Relationships
None

## JSON representation
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

