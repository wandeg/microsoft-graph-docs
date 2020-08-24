---
title: "managedDeviceModelsAndManufacturers resource type"
description: "Models and Manufactures meatadata for managed devices in the account"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# managedDeviceModelsAndManufacturers resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Models and Manufactures meatadata for managed devices in the account

## Properties

| Property            | Type              | Description                                             |
| :------------------ | :---------------- | :------------------------------------------------------ |
| deviceManufacturers | String collection | List of Manufactures for managed devices in the account |
| deviceModels        | String collection | List of Models for managed devices in the account       |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceManufacturers": ["String"],
  "deviceModels": ["String"]
}
```