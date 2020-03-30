---
title: "educationAssignmentPointsGrade resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationAssignmentPointsGrade resource type


Namespace: microsoft.graph




Inherits from [educationAssignmentGrade](../resources/educationassignmentgrade.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|gradedBy|[identitySet](../resources/identityset.md)| Inherited from [educationAssignmentGrade](../resources/educationassignmentgrade.md)|
|gradedDateTime|DateTimeOffset| Inherited from [educationAssignmentGrade](../resources/educationassignmentgrade.md)|
|points|Single||

## Relationships
None

## JSON representation
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

