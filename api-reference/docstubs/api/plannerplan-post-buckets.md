---
title: "Add buckets"
description: "Add buckets by posting to the buckets collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add buckets

Namespace: microsoft.graph

Add buckets by posting to the buckets collection.

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
POST /invitations/{invitationsId}/invitedUser/planner/plans/{plannerPlanId}/buckets/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [plannerBucket](../resources/plannerbucket.md) object.

The following table shows the properties that are required when you create the [plannerBucket](../resources/plannerbucket.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|
|orderHint|String|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and a [plannerBucket](../resources/plannerbucket.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/planner/plans/{plannerPlanId}/buckets/$ref
Content-Type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "name": "Name value",
  "planId": "Plan Id value",
  "orderHint": "Order Hint value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerbucket"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "2d045bbf-5bbf-2d04-bf5b-042dbf5b042d",
  "name": "Name value",
  "planId": "Plan Id value",
  "orderHint": "Order Hint value"
}
```

