---
title: "rubricLevel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# rubricLevel resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|description|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)|**TODO: Add Description**|
|levelId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.educationItemBody"
  },
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  }
}
```

