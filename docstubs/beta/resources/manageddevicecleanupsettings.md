---
title: "managedDeviceCleanupSettings resource type"
description: "Define the rule when the admin wants the devices to be cleaned up."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# managedDeviceCleanupSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Define the rule when the admin wants the devices to be cleaned up.

## Properties

| Property                               | Type   | Description                                              |
| :------------------------------------- | :----- | :------------------------------------------------------- |
| deviceInactivityBeforeRetirementInDays | String | Number of days when the device has not contacted Intune. |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```