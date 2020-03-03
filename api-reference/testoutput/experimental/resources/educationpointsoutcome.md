---
title: "educationPointsOutcome resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationPointsOutcome resource type


Namespace: microsoft.graph




Inherits from [educationOutcome](../resources/educationoutcome.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List educationPointsOutcomes](../api/educationpointsoutcome-list.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md) collection|List properties and relationships of the [educationPointsOutcome](../resources/educationpointsoutcome.md) objects.|
|[Get educationPointsOutcome](../api/educationpointsoutcome-get.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md)|Read properties and relationships of the [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Create educationPointsOutcome](../api/educationpointsoutcome-create.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md)|Create a new [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Delete educationPointsOutcome](../api/educationpointsoutcome-delete.md)|None|Deletes a [educationPointsOutcome](../resources/educationpointsoutcome.md).|
|[Update educationPointsOutcome](../api/educationpointsoutcome-update.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md)|Update the properties of a [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [educationOutcome](../resources/educationoutcome.md)|
|points|[educationAssignmentPointsGrade](../resources/educationassignmentpointsgrade.md)||
|publishedPoints|[educationAssignmentPointsGrade](../resources/educationassignmentpointsgrade.md)||

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

