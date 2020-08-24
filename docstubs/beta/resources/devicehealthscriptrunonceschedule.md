---
title: "deviceHealthScriptRunOnceSchedule resource type"
description: "Device health script run once schedule."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptRunOnceSchedule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device health script run once schedule.

## Properties

| Property | Type      | Description                                                                                                                                                                     |
| :------- | :-------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| date     | Date      | The date the script is scheduled to run. This collection can contain a maximum of 20 elements.                                                                                  |
| interval | Int32     | The x value of every x hours for hourly schedule, every x days for Daily Schedule, every x weeks for weekly schedule, every x months for Monthly Schedule. Valid values 1 to 23 |
| time     | TimeOfDay | At what time the script is scheduled to run. This collection can contain a maximum of 20 elements.                                                                              |
| useUtc   | Boolean   | Indicate if the time is Utc or client local time.                                                                                                                               |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptRunOnceSchedule",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunOnceSchedule",
  "date": "Date",
  "interval": "Int32",
  "time": "TimeOfDay",
  "useUtc": "Boolean"
}
```