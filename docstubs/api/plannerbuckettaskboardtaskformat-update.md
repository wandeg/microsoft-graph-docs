---
title: "Update plannerBucketTaskBoardTaskFormat"
description: "Update the properties of a plannerBucketTaskBoardTaskFormat object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerBucketTaskBoardTaskFormat

Namespace: microsoft.graph

Update the properties of a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.

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
PATCH /me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/bucketTaskBoardFormat
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.

The following table shows the properties that are required when you create the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|orderHint|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_plannerbuckettaskboardtaskformat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/tasks/{plannerTaskId}/bucketTaskBoardFormat
Content-type: application/json
Content-length: 110

{
  "@odata.type": "#microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "orderHint": "Order Hint value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 159

{
  "@odata.type": "#microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "id": "3acb4004-4004-3acb-0440-cb3a0440cb3a",
  "orderHint": "Order Hint value"
}
```

