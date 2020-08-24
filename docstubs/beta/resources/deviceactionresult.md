---
title: "deviceActionResult resource type"
description: "Device action result"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Device action result

## Properties

| Property            | Type           | Description                            |
| :------------------ | :------------- | :------------------------------------- |
| actionName          | String         | Action name                            |
| actionState         | String         | State of the action                    |
| lastUpdatedDateTime | DateTimeOffset | Time the action state was last updated |
| startDateTime       | DateTimeOffset | Time the action was initiated          |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceActionResult",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "lastUpdatedDateTime": "DateTimeOffset",
  "startDateTime": "DateTimeOffset"
}
```