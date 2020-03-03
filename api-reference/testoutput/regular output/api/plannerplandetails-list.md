---
title: "List plannerPlanDetailses"
description: "List properties and relationships of the plannerPlanDetails objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List plannerPlanDetailses

Namespace: microsoft.graph

List properties and relationships of the [plannerPlanDetails](../resources/plannerplandetails.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.plannerPlanDetails not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerPlanDetails](../resources/plannerplandetails.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerplandetails"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.plannerPlanDetails not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannerplandetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 599

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlanDetails",
      "id": "e46e20fd-20fd-e46e-fd20-6ee4fd206ee4",
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
  ]
}
```

