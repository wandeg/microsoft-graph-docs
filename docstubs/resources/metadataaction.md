---
title: "metadataAction resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# metadataAction resource type


Namespace: microsoft.graph




Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|metadataToAdd|[keyValuePair](../resources/keyvaluepair.md) collection||
|metadataToRemove|String collection||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.metadataAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.metadataAction",
  "metadataToRemove": [
    "String"
  ],
  "metadataToAdd": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```

