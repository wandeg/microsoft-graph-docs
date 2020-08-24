---
title: "allLicensedUsersAssignmentTarget resource type"
description: "Represents an assignment to all licensed users in the tenant."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# allLicensedUsersAssignmentTarget resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an assignment to all licensed users in the tenant.

## Properties

| Property                                   | Type   | Description                                                          |
| :----------------------------------------- | :----- | :------------------------------------------------------------------- |
| deviceAndAppManagementAssignmentFilterId   | String | The Id of the filter for the target assignment.                      |
| deviceAndAppManagementAssignmentFilterType | String | The type of filter of the target assignment i.e. Exclude or Include. |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.allLicensedUsersAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "none | include"
}
```