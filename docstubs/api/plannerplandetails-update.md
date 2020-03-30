---
title: "Update plannerPlanDetails"
description: "Update the properties of a plannerPlanDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update plannerPlanDetails

Namespace: microsoft.graph

Update the properties of a [plannerPlanDetails](../resources/plannerplandetails.md) object.

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
PATCH /me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/details
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [plannerPlanDetails](../resources/plannerplandetails.md) object.

The following table shows the properties that are required when you create the [plannerPlanDetails](../resources/plannerplandetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)||
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)||
|contextDetails|[plannerPlanContextDetailsCollection](../resources/plannerplancontextdetailscollection.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_plannerplandetails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/joinedGroups/{groupId}/planner/plans/{plannerPlanId}/details
Content-type: application/json
Content-length: 564

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
  },
  "contextDetails": {
    "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "e404f06f-f06f-e404-6ff0-04e46ff004e4",
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
```

