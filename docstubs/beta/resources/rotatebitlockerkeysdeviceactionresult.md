---
title: "rotateBitLockerKeysDeviceActionResult resource type"
description: "RotateBitLockerKeys device action result"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# rotateBitLockerKeysDeviceActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

RotateBitLockerKeys device action result

## Properties

| Property            | Type           | Description                            |
| :------------------ | :------------- | :------------------------------------- |
| actionName          | String         | Action name                            |
| actionState         | String         | State of the action                    |
| errorCode           | Int32          | RotateBitLockerKeys action error code  |
| lastUpdatedDateTime | DateTimeOffset | Time the action state was last updated |
| startDateTime       | DateTimeOffset | Time the action was initiated          |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.rotateBitLockerKeysDeviceActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.rotateBitLockerKeysDeviceActionResult",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "errorCode": "Int32",
  "lastUpdatedDateTime": "DateTimeOffset",
  "startDateTime": "DateTimeOffset"
}
```