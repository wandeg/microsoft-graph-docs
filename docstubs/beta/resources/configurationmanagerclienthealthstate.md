---
title: "configurationManagerClientHealthState resource type"
description: "Configuration manager client health state"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# configurationManagerClientHealthState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configuration manager client health state

## Properties

| Property         | Type           | Description                                                         |
| :--------------- | :------------- | :------------------------------------------------------------------ |
| errorCode        | Int32          | Error code for failed state.                                        |
| lastSyncDateTime | DateTimeOffset | Datetime for last sync with configuration manager management point. |
| state            | String         | Current configuration manager client state.                         |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "errorCode": "Int32",
  "lastSyncDateTime": "DateTimeOffset",
  "state": "unknown | installed | healthy | installFailed | updateFailed | communicationError"
}
```