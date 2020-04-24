---
title: "stringKeyAttributeMappingSourceValuePair resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# stringKeyAttributeMappingSourceValuePair resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|key|String|**TODO: Add Description**|
|value|[attributeMappingSource](../resources/attributemappingsource.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.stringKeyAttributeMappingSourceValuePair",
  "key": "String",
  "value": {
    "@odata.type": "microsoft.graph.attributeMappingSource",
    "expression": "String",
    "name": "String",
    "parameters": [
      {
        "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
      }
    ],
    "type": "String"
  }
}
```

