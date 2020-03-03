---
title: "rubricLevel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# rubricLevel resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|[educationItemBody](../resources/educationItemBody.md)||
|displayName|String||
|grading|[educationAssignmentGradeType](../resources/educationAssignmentGradeType.md)||
|levelId|String||

## Relationships
None

## JSON Representation
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

