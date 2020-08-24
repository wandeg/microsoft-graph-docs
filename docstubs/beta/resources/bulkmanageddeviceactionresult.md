---
title: "bulkManagedDeviceActionResult resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# bulkManagedDeviceActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property              | Type              | Description           |
| :-------------------- | :---------------- | :-------------------- |
| failedDeviceIds       | String collection | Failed devices        |
| notFoundDeviceIds     | String collection | Not found devices     |
| notSupportedDeviceIds | String collection | Not supported devices |
| successfulDeviceIds   | String collection | Successful devices    |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "failedDeviceIds": ["String"],
  "notFoundDeviceIds": ["String"],
  "notSupportedDeviceIds": ["String"],
  "successfulDeviceIds": ["String"]
}
```