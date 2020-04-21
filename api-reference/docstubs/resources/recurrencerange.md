---
title: "recurrenceRange resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# recurrenceRange resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|endDate|Date|**TODO: Add Description**|
|numberOfOccurrences|Int32|**TODO: Add Description**|
|recurrenceTimeZone|String|**TODO: Add Description**|
|startDate|Date|**TODO: Add Description**|
|type|recurrenceRangeType|**TODO: Add Description**. Possible values are: `endDate`, `noEnd`, `numbered`.|

## Relationships
None

## JSON representation
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

