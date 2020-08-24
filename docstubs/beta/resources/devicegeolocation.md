---
title: "deviceGeoLocation resource type"
description: "Device location"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceGeoLocation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device location

## Properties

| Property                 | Type           | Description                                          |
| :----------------------- | :------------- | :--------------------------------------------------- |
| altitude                 | Double         | Altitude, given in meters above sea level            |
| heading                  | Double         | Heading in degrees from true north                   |
| horizontalAccuracy       | Double         | Accuracy of longitude and latitude in meters         |
| lastCollectedDateTime    | DateTimeOffset | Time at which location was recorded, relative to UTC |
| lastCollectedDateTimeUtc | DateTimeOffset | Time at which location was recorded, relative to UTC |
| latitude                 | Double         | Latitude coordinate of the device's location         |
| longitude                | Double         | Longitude coordinate of the device's location        |
| speed                    | Double         | Speed the device is traveling in meters per second   |
| verticalAccuracy         | Double         | Accuracy of altitude in meters                       |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceGeoLocation",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceGeoLocation",
  "altitude": "Double",
  "heading": "Double",
  "horizontalAccuracy": "Double",
  "lastCollectedDateTime": "DateTimeOffset",
  "lastCollectedDateTimeUtc": "DateTimeOffset",
  "latitude": "Double",
  "longitude": "Double",
  "speed": "Double",
  "verticalAccuracy": "Double"
}
```