---
title: "osVersionCount resource type"
description: "Count of devices with malware for each OS version"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# osVersionCount resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Count of devices with malware for each OS version

## Properties

| Property           | Type           | Description                                                  |
| :----------------- | :------------- | :----------------------------------------------------------- |
| deviceCount        | Int32          | Count of devices with malware for the OS version             |
| lastUpdateDateTime | DateTimeOffset | The Timestamp of the last update for the device count in UTC |
| osVersion          | String         | OS version                                                   |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "deviceCount": "Int32",
  "lastUpdateDateTime": "DateTimeOffset",
  "osVersion": "String"
}
```