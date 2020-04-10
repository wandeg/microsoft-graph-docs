---
title: "Update plannerProgressTaskBoardTaskFormat"
description: "Update the properties of a plannerProgressTaskBoardTaskFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerProgressTaskBoardTaskFormat

Namespace: microsoft.graph

Update the properties of a [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/progressTaskBoardFormat
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object.

The following table shows the properties that are required when you create the [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerProgressTaskBoardTaskFormat](../resources/plannerprogresstaskboardtaskformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_plannerprogresstaskboardtaskformat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/progressTaskBoardFormat
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "orderHint": "Order Hint value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.plannerProgressTaskBoardTaskFormat",
  "id": "07f96f29-6f29-07f9-296f-f907296ff907",
  "orderHint": "Order Hint value"
}
```

