---
title: "locateDeviceActionResult resource type"
description: "Locate device action result"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# locateDeviceActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Locate device action result

## Properties

| Property            | Type                                                   | Description                            |
| :------------------ | :----------------------------------------------------- | :------------------------------------- |
| actionName          | String                                                 | Action name                            |
| actionState         | String                                                 | State of the action                    |
| deviceLocation      | [deviceGeoLocation](../resources/devicegeolocation.md) | device location                        |
| lastUpdatedDateTime | DateTimeOffset                                         | Time the action state was last updated |
| startDateTime       | DateTimeOffset                                         | Time the action was initiated          |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locateDeviceActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.locateDeviceActionResult",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "deviceLocation": {"@odata.type": "microsoft.graph.deviceGeoLocation"},
  "lastUpdatedDateTime": "DateTimeOffset",
  "startDateTime": "DateTimeOffset"
}
```