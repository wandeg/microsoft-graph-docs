---
title: "Get plannerPlanDetails"
description: "Read the properties and relationships of a plannerPlanDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get plannerPlanDetails

Namespace: microsoft.graph

Read the properties and relationships of a [plannerPlanDetails](../resources/plannerplandetails.md) object.

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
GET /invitations/{invitationsId}/invitedUser/planner/plans/{plannerPlanId}/details
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/planner/plans/{plannerPlanId}/details
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
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
}
```

