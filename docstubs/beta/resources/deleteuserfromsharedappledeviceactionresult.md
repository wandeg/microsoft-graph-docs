---
title: "deleteUserFromSharedAppleDeviceActionResult resource type"
description: "Delete user from shared apple device action result"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deleteUserFromSharedAppleDeviceActionResult resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Delete user from shared apple device action result

## Properties

| Property            | Type           | Description                                   |
| :------------------ | :------------- | :-------------------------------------------- |
| actionName          | String         | Action name                                   |
| actionState         | String         | State of the action                           |
| lastUpdatedDateTime | DateTimeOffset | Time the action state was last updated        |
| startDateTime       | DateTimeOffset | Time the action was initiated                 |
| userPrincipalName   | String         | User principal name of the user to be deleted |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deleteUserFromSharedAppleDeviceActionResult",
  "actionName": "String",
  "actionState": "none | pending | canceled | active | done | failed | notSupported",
  "lastUpdatedDateTime": "DateTimeOffset",
  "startDateTime": "DateTimeOffset",
  "userPrincipalName": "String"
}
```