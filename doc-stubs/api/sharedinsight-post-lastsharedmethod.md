---
title: "Add lastSharedMethod"
description: "Add lastSharedMethod by posting to the lastSharedMethod collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add lastSharedMethod

Namespace: microsoft.graph

Add lastSharedMethod by posting to the lastSharedMethod collection.

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
POST /users/{usersId}/insights/shared/{sharedInsightId}/lastSharedMethod/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [entity](../resources/entity.md) object.

The following table shows the properties that are required when you create the [entity](../resources/entity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and an [entity](../resources/entity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_entity_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/insights/shared/{sharedInsightId}/lastSharedMethod/$ref
Content-Type: application/json
Content-length: 48

{
  "@odata.type": "#microsoft.graph.entity"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.entity"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.entity",
  "id": "9851ab2b-ab2b-9851-2bab-51982bab5198"
}
```

