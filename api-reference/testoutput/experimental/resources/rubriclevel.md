---
title: "rubricLevel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# rubricLevel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|[educationItemBody](../resources/educationitembody.md)||
|displayName|String||
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)||
|levelId|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rubricLevel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rubricLevel",
  "levelId": "String",
  "displayName": "String",
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "String"
  },
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  }
}
```

