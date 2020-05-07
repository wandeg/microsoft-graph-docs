---
title: "hourlySchedule resource type"
description: "Hourly run schedule of a recurring device management script."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# hourlySchedule resource type


Namespace: microsoft.graph

Hourly run schedule of a recurring device management script.


Inherits from [runSchedule](../resources/runschedule.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|interval|Int32|Interval in number of hours|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.hourlySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.hourlySchedule",
  "interval": "Integer"
}
```

