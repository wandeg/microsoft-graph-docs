---
title: "userFeedback resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# userFeedback resource type


Namespace: microsoft.graph.callRecords

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|rating|userFeedbackRating|**TODO: Add Description**. Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|text|String|**TODO: Add Description**|
|tokens|[feedbackTokenSet](../resources/callrecords-feedbacktokenset.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.userFeedback"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.userFeedback",
  "text": "String",
  "rating": "String",
  "tokens": {
    "@odata.type": "microsoft.graph.callRecords.feedbackTokenSet"
  }
}
```

