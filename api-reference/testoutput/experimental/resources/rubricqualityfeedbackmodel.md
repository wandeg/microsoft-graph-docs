---
title: "rubricQualityFeedbackModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# rubricQualityFeedbackModel resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[educationItemBody](../resources/educationItemBody.md)||
|qualityId|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rubricQualityFeedbackModel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.rubricQualityFeedbackModel",
  "qualityId": "String",
  "feedback": {
    "@odata.type": "microsoft.graph.educationItemBody",
    "contentType": "String",
    "content": "String"
  }
}
```

