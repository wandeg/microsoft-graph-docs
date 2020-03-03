---
title: "recurrenceRange resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# recurrenceRange resource type



## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDate|Date||
|numberOfOccurrences|Int32||
|recurrenceTimeZone|String||
|startDate|Date||
|type|Enumeration|. Possible values are: `endDate`, `noEnd`, `numbered`.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.recurrenceRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.recurrenceRange",
  "type": "String",
  "startDate": "Date",
  "endDate": "Date",
  "recurrenceTimeZone": "String",
  "numberOfOccurrences": 1024
}
```

