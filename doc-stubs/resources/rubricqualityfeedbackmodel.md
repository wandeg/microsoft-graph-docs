---
title: "rubricQualityFeedbackModel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# rubricQualityFeedbackModel resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|feedback|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|qualityId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
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
    "@odata.type": "microsoft.graph.educationItemBody"
  }
}
```

