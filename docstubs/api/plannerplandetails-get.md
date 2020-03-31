---
title: "Get plannerPlanDetails"
description: "Read properties and relationships of the plannerPlanDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get plannerPlanDetails

Namespace: microsoft.graph

Read properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) object.

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
GET /me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/details
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/details
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": {
    "@odata.type": "#microsoft.graph.plannerPlanDetails",
    "id": "7cb1a5ec-a5ec-7cb1-eca5-b17ceca5b17c",
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
    },
    "contextDetails": {
      "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
    }
  }
}
```

