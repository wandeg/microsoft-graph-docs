---
title: "updateWindowsDeviceAccountActionParameter resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# updateWindowsDeviceAccountActionParameter resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property                         | Type                                                         | Description |
| :------------------------------- | :----------------------------------------------------------- | :---------- |
| calendarSyncEnabled              | Boolean                                                      |             |
| deviceAccount                    | [windowsDeviceAccount](../resources/windowsdeviceaccount.md) |             |
| deviceAccountEmail               | String                                                       |             |
| exchangeServer                   | String                                                       |             |
| passwordRotationEnabled          | Boolean                                                      |             |
| sessionInitiationProtocalAddress | String                                                       |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.updateWindowsDeviceAccountActionParameter",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.updateWindowsDeviceAccountActionParameter",
  "calendarSyncEnabled": "Boolean",
  "deviceAccount": {"@odata.type": "microsoft.graph.windowsDeviceAccount"},
  "deviceAccountEmail": "String",
  "exchangeServer": "String",
  "passwordRotationEnabled": "Boolean",
  "sessionInitiationProtocalAddress": "String"
}
```