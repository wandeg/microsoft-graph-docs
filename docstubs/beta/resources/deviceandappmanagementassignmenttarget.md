---
title: "deviceAndAppManagementAssignmentTarget resource type"
description: "Base type for assignment targets."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# deviceAndAppManagementAssignmentTarget resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Base type for assignment targets.

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
  "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementAssignmentTarget",
  "deviceAndAppManagementAssignmentFilterId": "String",
  "deviceAndAppManagementAssignmentFilterType": "none | include"
}
```