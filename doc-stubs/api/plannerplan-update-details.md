---
title: "Update details"
description: "Update the properties of a details object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update details

Namespace: microsoft.graph

Update the properties of a details object.

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
PATCH /users/{usersId}/planner/plans/{plannerPlanId}/details
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerPlanDetails](../resources/plannerplandetails.md) object.

The following table shows the properties that are required when you create the [plannerPlanDetails](../resources/plannerplandetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)|**TODO: Add Description**|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_details"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}/planner/plans/{plannerPlanId}/details
Content-Type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  },
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  }
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
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "5f2195c4-95c4-5f21-c495-215fc495215f",
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  },
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  }
}
```

