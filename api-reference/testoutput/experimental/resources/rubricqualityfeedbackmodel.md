---
title: "rubricQualityFeedbackModel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# rubricQualityFeedbackModel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[educationItemBody](../resources/educationitembody.md)||
|qualityId|String||

## Relationships
None

## JSON representation
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

