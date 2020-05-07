---
title: "Update bucketTaskBoardFormat"
description: "Update the properties of a bucketTaskBoardFormat object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update bucketTaskBoardFormat

Namespace: microsoft.graph

Update the properties of a bucketTaskBoardFormat object.

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
PATCH /users/{usersId}/planner/tasks/{plannerTaskId}/bucketTaskBoardFormat
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object.

The following table shows the properties that are required when you create the [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|orderHint|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_buckettaskboardformat"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/users/{usersId}/planner/tasks/{plannerTaskId}/bucketTaskBoardFormat
Content-Type: application/json
Content-length: 100

{
  "@odata.type": "#microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "orderHint": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "id": "bc569830-9830-bc56-3098-56bc309856bc",
  "orderHint": "String"
}
```

