---
title: "assignmentReviewSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# assignmentReviewSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|durationInDays|Int32||
|isEnabled|Boolean||
|recurrenceType|String||
|reviewers|[userSet](../resources/userset.md) collection||
|reviewerType|String||
|startDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentReviewSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentReviewSettings",
  "isEnabled": true,
  "recurrenceType": "String",
  "reviewerType": "String",
  "startDateTime": "String (timestamp)",
  "durationInDays": 1024,
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.singleUser",
      "isBackup": true,
      "id": "String",
      "description": "String"
    }
  ]
}
```

