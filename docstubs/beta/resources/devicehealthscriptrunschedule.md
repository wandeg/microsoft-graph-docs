---
title: "deviceHealthScriptRunSchedule resource type"
description: "Base type of Device health script run schedule."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceHealthScriptRunSchedule resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Base type of Device health script run schedule.

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
  "@odata.type": "microsoft.graph.deviceHealthScriptRunSchedule",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSchedule",
  "interval": "Int32"
}
```