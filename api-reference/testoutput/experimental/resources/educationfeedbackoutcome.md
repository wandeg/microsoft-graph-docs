---
title: "educationFeedbackOutcome resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationFeedbackOutcome resource type




Inherits from [educationOutcome](../resources/educationOutcome.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationFeedbackOutcomes](../api/educationfeedbackoutcome-list.md)|[educationFeedbackOutcome](../resources/educationFeedbackOutcome.md) collection|List properties and relationships of the [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) objects.|
|[Get educationFeedbackOutcome](../api/educationfeedbackoutcome-get.md)|[educationFeedbackOutcome](../resources/educationFeedbackOutcome.md)|Read properties and relationships of the [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) object.|
|[Create educationFeedbackOutcome](../api/educationfeedbackoutcome-create.md)|[educationFeedbackOutcome](../resources/educationFeedbackOutcome.md)|Create a new [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) object.|
|[Delete educationFeedbackOutcome](../api/educationfeedbackoutcome-delete.md)|None|Deletes a [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md).|
|[Update educationFeedbackOutcome](../api/educationfeedbackoutcome-update.md)|[educationFeedbackOutcome](../resources/educationFeedbackOutcome.md)|Update the properties of a [educationFeedbackOutcome](../resources/educationfeedbackoutcome.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[educationFeedback](../resources/educationFeedback.md)||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|publishedFeedback|[educationFeedback](../resources/educationFeedback.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationFeedbackOutcome",
  "baseType": "microsoft.graph.educationOutcome",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationFeedbackOutcome",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "feedback": {
    "@odata.type": "microsoft.graph.educationFeedback"
  },
  "publishedFeedback": {
    "@odata.type": "microsoft.graph.educationFeedback"
  }
}
```

