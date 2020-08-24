---
title: "deviceHealthScriptHourlySchedule resource type"
description: "Type of Device health script hourly schedule."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptHourlySchedule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Type of Device health script hourly schedule.

## Properties

| Property | Type  | Description                                                                                                                                                                     |
| :------- | :---- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| interval | Int32 | The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule. Valid values 1 to 23 |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptHourlySchedule",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptHourlySchedule",
  "interval": "Int32"
}
```