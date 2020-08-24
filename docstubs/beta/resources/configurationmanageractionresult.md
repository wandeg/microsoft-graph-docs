---
title: "configurationManagerActionResult resource type"
description: "Result of the ConfigurationManager action"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# configurationManagerActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Result of the ConfigurationManager action

## Properties

| Property             | Type           | Description                                            |
| :------------------- | :------------- | :----------------------------------------------------- |
| actionDeliveryStatus | String         | State of the action being delivered to on-prem server  |
| actionName           | String         | Action name                                            |
| actionState          | String         | State of the action                                    |
| errorCode            | Int32          | Error code of Configuration Manager action from client |
| lastUpdatedDateTime  | DateTimeOffset | Time the action state was last updated                 |
| startDateTime        | DateTimeOffset | Time the action was initiated                          |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.configurationManagerActionResult",
  "actionDeliveryStatus": "unknown | pendingDelivery | deliveredToConnectorService | failedToDeliverToConnectorService | deliveredToOnPremisesServer",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "errorCode": "Int32",
  "lastUpdatedDateTime": "DateTimeOffset",
  "startDateTime": "DateTimeOffset"
}
```