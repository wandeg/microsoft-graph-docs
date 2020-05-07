---
title: "attributeMapping resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attributeMapping resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultValue|String|**TODO: Add Description**|
|exportMissingReferences|Boolean|**TODO: Add Description**|
|flowBehavior|attributeFlowBehavior|**TODO: Add Description**. Possible values are: `FlowWhenChanged`, `FlowAlways`.|
|flowType|attributeFlowType|**TODO: Add Description**. Possible values are: `Always`, `ObjectAddOnly`, `MultiValueAddOnly`.|
|matchingPriority|Int32|**TODO: Add Description**|
|source|[attributeMappingSource](../resources/attributemappingsource.md)|**TODO: Add Description**|
|targetAttributeName|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attributeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attributeMapping",
  "defaultValue": "String",
  "exportMissingReferences": "Boolean",
  "flowBehavior": "String",
  "flowType": "String",
  "matchingPriority": "Integer",
  "source": {
    "@odata.type": "microsoft.graph.attributeMappingSource"
  },
  "targetAttributeName": "String"
}
```

