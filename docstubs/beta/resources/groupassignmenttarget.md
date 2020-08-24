---
title: "groupAssignmentTarget resource type"
description: "Represents an assignment to a group."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# groupAssignmentTarget resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents an assignment to a group.

## Properties

| Property                                   | Type   | Description                                                          |
| :----------------------------------------- | :----- | :------------------------------------------------------------------- |
| deviceAndAppManagementAssignmentFilterId   | String | The Id of the filter for the target assignment.                      |
| deviceAndAppManagementAssignmentFilterType | String | The type of filter of the target assignment i.e. Exclude or Include. |
| groupId                                    | String | The group Id that is the target of the assignment.                   |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "none | include",
  "groupId": "String"
}
```