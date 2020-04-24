---
title: "standardTimeZoneOffset resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# standardTimeZoneOffset resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|dayOccurrence|Int32|**TODO: Add Description**|
|dayOfWeek|dayOfWeek|**TODO: Add Description**. Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.|
|month|Int32|**TODO: Add Description**|
|time|TimeOfDay|**TODO: Add Description**|
|year|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.standardTimeZoneOffset"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.standardTimeZoneOffset",
  "time": "String (time of day)",
  "dayOccurrence": 1024,
  "dayOfWeek": "String",
  "month": 1024,
  "year": 1024
}
```

