---
title: "revokeAppleVppLicensesActionResult resource type"
description: "Revoke Apple Vpp licenses action result"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# revokeAppleVppLicensesActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Revoke Apple Vpp licenses action result

## Properties

| Property            | Type           | Description                                              |
| :------------------ | :------------- | :------------------------------------------------------- |
| actionName          | String         | Action name                                              |
| actionState         | String         | State of the action                                      |
| failedLicensesCount | Int32          | Total number of Apple Vpp licenses that failed to revoke |
| lastUpdatedDateTime | DateTimeOffset | Time the action state was last updated                   |
| startDateTime       | DateTimeOffset | Time the action was initiated                            |
| totalLicensesCount  | Int32          | Total number of Apple Vpp licenses associated            |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "failedLicensesCount": "Int32",
  "lastUpdatedDateTime": "DateTimeOffset",
  "startDateTime": "DateTimeOffset",
  "totalLicensesCount": "Int32"
}
```