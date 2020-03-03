---
title: "userFeedback resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userFeedback resource type


Namespace: microsoft.graph.callRecords



## Properties
|Property|Type|Description|
|:---|:---|:---|
|rating|Enumeration|. Possible values are: `notRated`, `bad`, `poor`, `fair`, `good`, `excellent`, `unknownFutureValue`.|
|text|String||
|tokens|[feedbackTokenSet](../resources/callrecords-feedbacktokenset.md)||

## Relationships
None

## JSON Representation
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

