---
title: "labelingOptions resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# labelingOptions resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentMethod|Enumeration| Possible values are: `standard`, `privileged`, `auto`.|
|downgradeJustification|[downgradeJustification](../resources/downgradejustification.md)||
|extendedProperties|[keyValuePair](../resources/keyvaluepair.md) collection||
|labelId|Guid||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.labelingOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.labelingOptions",
  "labelId": "Guid",
  "assignmentMethod": "String",
  "downgradeJustification": {
    "@odata.type": "microsoft.graph.downgradeJustification",
    "justificationMessage": "String",
    "isDowngradeJustified": true
  },
  "extendedProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```

