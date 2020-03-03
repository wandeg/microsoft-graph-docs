---
title: "educationRubricOutcome resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationRubricOutcome resource type


Namespace: microsoft.graph




Inherits from [educationOutcome](../resources/educationoutcome.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationRubricOutcomes](../api/educationrubricoutcome-list.md)|[educationRubricOutcome](../resources/educationrubricoutcome.md) collection|List properties and relationships of the [educationRubricOutcome](../resources/educationrubricoutcome.md) objects.|
|[Get educationRubricOutcome](../api/educationrubricoutcome-get.md)|[educationRubricOutcome](../resources/educationrubricoutcome.md)|Read properties and relationships of the [educationRubricOutcome](../resources/educationrubricoutcome.md) object.|
|[Create educationRubricOutcome](../api/educationrubricoutcome-create.md)|[educationRubricOutcome](../resources/educationrubricoutcome.md)|Create a new [educationRubricOutcome](../resources/educationrubricoutcome.md) object.|
|[Delete educationRubricOutcome](../api/educationrubricoutcome-delete.md)|None|Deletes a [educationRubricOutcome](../resources/educationrubricoutcome.md).|
|[Update educationRubricOutcome](../api/educationrubricoutcome-update.md)|[educationRubricOutcome](../resources/educationrubricoutcome.md)|Update the properties of a [educationRubricOutcome](../resources/educationrubricoutcome.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|publishedRubricQualityFeedback|[rubricQualityFeedbackModel](../resources/rubricqualityfeedbackmodel.md) collection||
|publishedRubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](../resources/rubricqualityselectedcolumnmodel.md) collection||
|rubricQualityFeedback|[rubricQualityFeedbackModel](../resources/rubricqualityfeedbackmodel.md) collection||
|rubricQualitySelectedLevels|[rubricQualitySelectedColumnModel](../resources/rubricqualityselectedcolumnmodel.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationRubricOutcome",
  "baseType": "microsoft.graph.educationOutcome",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationRubricOutcome",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "rubricQualityFeedback": [
    {
      "@odata.type": "microsoft.graph.rubricQualityFeedbackModel"
    }
  ],
  "rubricQualitySelectedLevels": [
    {
      "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"
    }
  ],
  "publishedRubricQualityFeedback": [
    {
      "@odata.type": "microsoft.graph.rubricQualityFeedbackModel"
    }
  ],
  "publishedRubricQualitySelectedLevels": [
    {
      "@odata.type": "microsoft.graph.rubricQualitySelectedColumnModel"
    }
  ]
}
```

