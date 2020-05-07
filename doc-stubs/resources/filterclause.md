---
title: "filterClause resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# filterClause resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|operatorName|String|**TODO: Add Description**|
|sourceOperandName|String|**TODO: Add Description**|
|targetOperand|[filterOperand](../resources/filteroperand.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.filterClause"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.filterClause",
  "operatorName": "String",
  "sourceOperandName": "String",
  "targetOperand": {
    "@odata.type": "microsoft.graph.filterOperand"
  }
}
```

