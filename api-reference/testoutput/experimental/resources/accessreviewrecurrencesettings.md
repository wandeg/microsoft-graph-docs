---
title: "accessReviewRecurrenceSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# accessReviewRecurrenceSettings resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|durationInDays|Int32||
|recurrenceCount|Int32||
|recurrenceEndType|String||
|recurrenceType|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewRecurrenceSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewRecurrenceSettings",
  "recurrenceType": "String",
  "recurrenceEndType": "String",
  "durationInDays": 1024,
  "recurrenceCount": 1024
}
```

