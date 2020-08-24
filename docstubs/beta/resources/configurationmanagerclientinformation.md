---
title: "configurationManagerClientInformation resource type"
description: "Configuration Manager client information synced from SCCM"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# configurationManagerClientInformation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configuration Manager client information synced from SCCM

## Properties

| Property         | Type    | Description                                           |
| :--------------- | :------ | :---------------------------------------------------- |
| clientIdentifier | String  | Configuration Manager Client Id from SCCM             |
| isBlocked        | Boolean | Configuration Manager Client blocked status from SCCM |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": "Boolean"
}
```