---
title: "labelingOptions resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# labelingOptions resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignmentMethod|assignmentMethod|**TODO: Add Description**. Possible values are: `standard`, `privileged`, `auto`.|
|downgradeJustification|[downgradeJustification](../resources/downgradejustification.md)|**TODO: Add Description**|
|extendedProperties|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|labelId|Guid|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.downgradeJustification"
  },
  "extendedProperties": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```

