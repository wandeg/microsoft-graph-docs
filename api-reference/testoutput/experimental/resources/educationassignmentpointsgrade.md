---
title: "educationAssignmentPointsGrade resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationAssignmentPointsGrade resource type




Inherits from [educationAssignmentGrade](../resources/educationAssignmentGrade.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gradedBy|[identitySet](../resources/identitySet.md)| Inherited from [educationAssignmentGrade](../resources/educationAssignmentGrade.md)|
|gradedDateTime|DateTimeOffset| Inherited from [educationAssignmentGrade](../resources/educationAssignmentGrade.md)|
|points|Single||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationAssignmentPointsGrade",
  "gradedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "String",
      "displayName": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "gradedDateTime": "String (timestamp)",
  "points": "Single"
}
```

