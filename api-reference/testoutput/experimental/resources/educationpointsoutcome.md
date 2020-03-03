---
title: "educationPointsOutcome resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationPointsOutcome resource type




Inherits from [educationOutcome](../resources/educationOutcome.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationPointsOutcomes](../api/educationpointsoutcome-list.md)|[educationPointsOutcome](../resources/educationPointsOutcome.md) collection|List properties and relationships of the [educationPointsOutcome](../resources/educationpointsoutcome.md) objects.|
|[Get educationPointsOutcome](../api/educationpointsoutcome-get.md)|[educationPointsOutcome](../resources/educationPointsOutcome.md)|Read properties and relationships of the [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Create educationPointsOutcome](../api/educationpointsoutcome-create.md)|[educationPointsOutcome](../resources/educationPointsOutcome.md)|Create a new [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Delete educationPointsOutcome](../api/educationpointsoutcome-delete.md)|None|Deletes a [educationPointsOutcome](../resources/educationpointsoutcome.md).|
|[Update educationPointsOutcome](../api/educationpointsoutcome-update.md)|[educationPointsOutcome](../resources/educationPointsOutcome.md)|Update the properties of a [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationOutcome.md)|
|points|[educationAssignmentPointsGrade](../resources/educationAssignmentPointsGrade.md)||
|publishedPoints|[educationAssignmentPointsGrade](../resources/educationAssignmentPointsGrade.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "microsoft.graph.educationOutcome",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationPointsOutcome",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "points": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
  },
  "publishedPoints": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
  }
}
```

