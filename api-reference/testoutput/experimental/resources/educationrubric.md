---
title: "educationRubric resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationRubric resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationRubric](../api/educationrubric-get.md)|[educationRubric](../resources/educationRubric.md)|Read properties and relationships of the [educationRubric](../resources/educationrubric.md) object.|
|[Delete educationRubric](../api/educationrubric-delete.md)|None|Deletes a [educationRubric](../resources/educationrubric.md).|
|[Update educationRubric](../api/educationrubric-update.md)|[educationRubric](../resources/educationRubric.md)|Update the properties of a [educationRubric](../resources/educationrubric.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identitySet.md)||
|createdDateTime|DateTimeOffset||
|description|[educationItemBody](../resources/educationItemBody.md)||
|displayName|String||
|grading|[educationAssignmentGradeType](../resources/educationAssignmentGradeType.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)||
|lastModifiedDateTime|DateTimeOffset||
|levels|[rubricLevel](../resources/rubricLevel.md) collection||
|qualities|[rubricQuality](../resources/rubricQuality.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationRubric",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationRubric",
  "id": "String (identifier)",
  "displayName": "String",
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody"
  },
  "qualities": [
    {
      "@odata.type": "microsoft.graph.rubricQuality"
    }
  ],
  "levels": [
    {
      "@odata.type": "microsoft.graph.rubricLevel"
    }
  ],
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```

