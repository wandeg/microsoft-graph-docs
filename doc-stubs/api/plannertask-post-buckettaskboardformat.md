---
title: "Create bucketTaskBoardFormat"
description: "Create a new bucketTaskBoardFormat object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create bucketTaskBoardFormat

Namespace: microsoft.graph

Create a new bucketTaskBoardFormat object.

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
POST /users/{usersId}/planner/tasks/{plannerTaskId}/bucketTaskBoardFormat
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

If successful, this method returns a `201 Created` response code and a [plannerBucketTaskBoardTaskFormat](../resources/plannerbuckettaskboardtaskformat.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerbuckettaskboardtaskformat_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/planner/tasks/{plannerTaskId}/bucketTaskBoardFormat
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
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerbuckettaskboardtaskformat"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerBucketTaskBoardTaskFormat",
  "id": "7db5e5c7-e5c7-7db5-c7e5-b57dc7e5b57d",
  "orderHint": "String"
}
```

