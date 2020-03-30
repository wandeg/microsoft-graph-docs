---
title: "rubricQuality resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# rubricQuality resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|criteria|[rubricCriterion](../resources/rubriccriterion.md) collection||
|description|[educationItemBody](../resources/educationitembody.md)||
|displayName|String||
|qualityId|String||
|weight|Single||

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

