---
title: "attributeMapping resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# attributeMapping resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultValue|String||
|exportMissingReferences|Boolean||
|flowBehavior|Enumeration|. Possible values are: `FlowWhenChanged`, `FlowAlways`.|
|flowType|Enumeration|. Possible values are: `Always`, `ObjectAddOnly`, `MultiValueAddOnly`.|
|matchingPriority|Int32||
|source|[attributeMappingSource](../resources/attributemappingsource.md)||
|targetAttributeName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attributeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeMapping",
  "defaultValue": "String",
  "exportMissingReferences": true,
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": 1024,
  "source": {
    "@odata.type": "microsoft.graph.attributeMappingSource",
    "expression": "String",
    "name": "String",
    "parameters": [
      {
        "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair",
        "key": "String",
        "value": {
          "@odata.type": "microsoft.graph.attributeMappingSource",
          "type": "String"
        }
      }
    ]
  },
  "targetAttributeName": "String"
}
```

