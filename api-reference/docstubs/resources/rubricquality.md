---
title: "rubricQuality resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# rubricQuality resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|criteria|[rubricCriterion](../resources/rubriccriterion.md) collection|**TODO: Add Description**|
|description|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|qualityId|String|**TODO: Add Description**|
|weight|Single|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rubricQuality"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rubricQuality",
  "qualityId": "String",
  "displayName": "String",
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "String"
  },
  "weight": "Single",
  "criteria": [
    {
      "@odata.type": "microsoft.graph.rubricCriterion"
    }
  ]
}
```

