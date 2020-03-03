---
title: "educationAssignmentGrade resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# educationAssignmentGrade resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|gradedBy|[identitySet](../resources/identitySet.md)||
|gradedDateTime|DateTimeOffset||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationAssignmentGrade"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationAssignmentGrade",
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
  "gradedDateTime": "String (timestamp)"
}
```

