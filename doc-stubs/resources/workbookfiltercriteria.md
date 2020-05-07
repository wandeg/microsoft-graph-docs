---
title: "workbookFilterCriteria resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# workbookFilterCriteria resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|color|String|**TODO: Add Description**|
|criterion1|String|**TODO: Add Description**|
|criterion2|String|**TODO: Add Description**|
|dynamicCriteria|String|**TODO: Add Description**|
|filterOn|String|**TODO: Add Description**|
|icon|[workbookIcon](../resources/workbookicon.md)|**TODO: Add Description**|
|operator|String|**TODO: Add Description**|
|values|[Json](../resources/json.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.workbookFilterCriteria",
  "color": "String",
  "criterion1": "String",
  "criterion2": "String",
  "dynamicCriteria": "String",
  "filterOn": "String",
  "icon": {
    "@odata.type": "microsoft.graph.workbookIcon"
  },
  "operator": "String",
  "values": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

