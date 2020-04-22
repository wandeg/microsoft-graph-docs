---
title: "List planner"
description: "Get the plannerUsers from the planner navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List planner

Namespace: microsoft.graph

Get the plannerUsers from the planner navigation property.

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
GET /me/planner
GET /users/{usersId}/planner
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
If successful, this method returns a `200 OK` response code and a collection of [plannerUser](../resources/planneruser.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_planneruser"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/planner
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.planneruser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerUser",
      "id": "d2ad66a8-66a8-d2ad-a866-add2a866add2",
      "favoritePlanReferences": {
        "@odata.type": "microsoft.graph.plannerFavoritePlanReferenceCollection"
      },
      "recentPlanReferences": {
        "@odata.type": "microsoft.graph.plannerRecentPlanReferenceCollection"
      }
    }
  ]
}
```

