---
title: "educationAssignmentPointsGrade resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationAssignmentPointsGrade resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [educationAssignmentGrade](../resources/educationassignmentgrade.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gradedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [educationAssignmentGrade](../resources/educationassignmentgrade.md)|
|gradedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [educationAssignmentGrade](../resources/educationassignmentgrade.md)|
|points|Single|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationAssignmentPointsGrade",
  "gradedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "gradedDateTime": "String (timestamp)",
  "points": "Single"
}
```

