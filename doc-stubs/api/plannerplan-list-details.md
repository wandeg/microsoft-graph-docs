---
title: "List details"
description: "Get the plannerPlanDetails from the details navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List details

Namespace: microsoft.graph

Get the plannerPlanDetails from the details navigation property.

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
GET /users/{usersId}/planner/plans/{plannerPlanId}/details
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [plannerPlanDetails](../resources/plannerplandetails.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/planner/plans/{plannerPlanId}/details
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannerplandetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlanDetails",
      "id": "7393a5c9-a5c9-7393-c9a5-9373c9a59373",
      "sharedWith": {
        "@odata.type": "microsoft.graph.plannerUserIds"
      },
      "categoryDescriptions": {
        "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
      },
      "contextDetails": {
        "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
      }
    }
  ]
}
```

