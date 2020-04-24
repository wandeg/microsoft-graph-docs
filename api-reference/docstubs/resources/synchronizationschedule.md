---
title: "synchronizationSchedule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# synchronizationSchedule resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expiration|DateTimeOffset|**TODO: Add Description**|
|interval|Duration|**TODO: Add Description**|
|state|synchronizationScheduleState|**TODO: Add Description**. Possible values are: `Active`, `Disabled`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.synchronizationSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.synchronizationSchedule",
  "expiration": "String (timestamp)",
  "interval": "String (duration)",
  "state": "String"
}
```

