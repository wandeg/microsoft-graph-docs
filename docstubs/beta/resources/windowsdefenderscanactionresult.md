---
title: "windowsDefenderScanActionResult resource type"
description: "Windows Defender last scan result"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# windowsDefenderScanActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows Defender last scan result

## Properties

| Property            | Type           | Description                              |
| :------------------ | :------------- | :--------------------------------------- |
| actionName          | String         | Action name                              |
| actionState         | String         | State of the action                      |
| lastUpdatedDateTime | DateTimeOffset | Time the action state was last updated   |
| scanType            | String         | Scan type either full scan or quick scan |
| startDateTime       | DateTimeOffset | Time the action was initiated            |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDefenderScanActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsDefenderScanActionResult",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "lastUpdatedDateTime": "DateTimeOffset",
  "scanType": "String",
  "startDateTime": "DateTimeOffset"
}
```