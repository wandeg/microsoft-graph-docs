---
title: "deviceExchangeAccessStateSummary resource type"
description: "Device Exchange Access State summary"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceExchangeAccessStateSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device Exchange Access State summary

## Properties

| Property               | Type  | Description                                                               |
| :--------------------- | :---- | :------------------------------------------------------------------------ |
| allowedDeviceCount     | Int32 | Total count of devices with Exchange Access State: Allowed.               |
| blockedDeviceCount     | Int32 | Total count of devices with Exchange Access State: Blocked.               |
| quarantinedDeviceCount | Int32 | Total count of devices with Exchange Access State: Quarantined.           |
| unavailableDeviceCount | Int32 | Total count of devices for which no Exchange Access State could be found. |
| unknownDeviceCount     | Int32 | Total count of devices with Exchange Access State: Unknown.               |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
  "allowedDeviceCount": "Int32",
  "blockedDeviceCount": "Int32",
  "quarantinedDeviceCount": "Int32",
  "unavailableDeviceCount": "Int32",
  "unknownDeviceCount": "Int32"
}
```