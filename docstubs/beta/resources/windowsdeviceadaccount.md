---
title: "windowsDeviceADAccount resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# windowsDeviceADAccount resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property   | Type   | Description |
| :--------- | :----- | :---------- |
| domainName | String |             |
| password   | String |             |
| userName   | String |             |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsDeviceADAccount",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.windowsDeviceADAccount",
  "domainName": "String",
  "password": "String",
  "userName": "String"
}
```