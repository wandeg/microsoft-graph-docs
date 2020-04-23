---
title: "Create details"
description: "Create a new details object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create details

Namespace: microsoft.graph

Create a new details object.

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
POST /invitations/{invitationsId}/invitedUser/planner/plans/{plannerPlanId}/details
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [plannerPlanDetails](../resources/plannerplandetails.md) object.

The following table shows the properties that are required when you create the [plannerPlanDetails](../resources/plannerplandetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)|**TODO: Add Description**|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerplandetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/planner/plans/{plannerPlanId}/details
Content-Type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  },
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions",
    "category1": "Category1 value",
    "category2": "Category2 value",
    "category3": "Category3 value",
    "category4": "Category4 value",
    "category5": "Category5 value",
    "category6": "Category6 value"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerplandetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "20c66712-6712-20c6-1267-c6201267c620",
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  },
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions",
    "category1": "Category1 value",
    "category2": "Category2 value",
    "category3": "Category3 value",
    "category4": "Category4 value",
    "category5": "Category5 value",
    "category6": "Category6 value"
  }
}
```

