---
title: "windowsDeviceAzureADAccount resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# windowsDeviceAzureADAccount resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property          | Type   | Description |
| :---------------- | :----- | :---------- |
| password          | String |             |
| userPrincipalName | String |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceAzureADAccount",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsDeviceAzureADAccount",
  "password": "String",
  "userPrincipalName": "String"
}
```