---
title: "metadataAction resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# metadataAction resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [informationProtectionAction](../resources/informationprotectionaction.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|metadataToAdd|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|
|metadataToRemove|String collection|**TODO: Add Description**|

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

