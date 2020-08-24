---
title: "loggedOnUser resource type"
description: "Logged On User"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# loggedOnUser resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Logged On User

## Properties

| Property          | Type           | Description                 |
| :---------------- | :------------- | :-------------------------- |
| lastLogOnDateTime | DateTimeOffset | Date time when user logs on |
| userId            | String         | User id                     |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "lastLogOnDateTime": "DateTimeOffset",
  "userId": "String"
}
```