---
title: "Create assignedToTaskBoardFormat"
description: "Create a new assignedToTaskBoardFormat object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create assignedToTaskBoardFormat

Namespace: microsoft.graph

Create a new assignedToTaskBoardFormat object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/assignedToTaskBoardFormat
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object.

The following table shows the properties that are required when you create the [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|unassignedOrderHint|String|**TODO: Add Description**|
|orderHintsByAssignee|[plannerOrderHintsByAssignee](../resources/plannerorderhintsbyassignee.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [plannerAssignedToTaskBoardTaskFormat](../resources/plannerassignedtotaskboardtaskformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerassignedtotaskboardtaskformat_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/assignedToTaskBoardFormat
Content-Type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "unassignedOrderHint": "Unassigned Order Hint value",
  "orderHintsByAssignee": {
    "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerassignedtotaskboardtaskformat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerAssignedToTaskBoardTaskFormat",
  "id": "b0e2bb24-bb24-b0e2-24bb-e2b024bbe2b0",
  "unassignedOrderHint": "Unassigned Order Hint value",
  "orderHintsByAssignee": {
    "@odata.type": "microsoft.graph.plannerOrderHintsByAssignee"
  }
}
```

