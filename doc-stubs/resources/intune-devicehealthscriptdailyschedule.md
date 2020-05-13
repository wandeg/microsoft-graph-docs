---
title: "deviceHealthScriptDailySchedule resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceHealthScriptDailySchedule resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceHealthScriptTimeSchedule](../resources/devicehealthscripttimeschedule.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|interval|Int32|**TODO: Add Description** Inherited from [deviceHealthScriptRunSchedule](../resources/intune-devicehealthscriptrunschedule.md)|
|time|TimeOfDay|**TODO: Add Description** Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devicehealthscripttimeschedule.md)|
|useUtc|Boolean|**TODO: Add Description** Inherited from [deviceHealthScriptTimeSchedule](../resources/intune-devicehealthscripttimeschedule.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptDailySchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptDailySchedule",
  "interval": "Integer",
  "useUtc": "Boolean",
  "time": "String (time of day)"
}
```

