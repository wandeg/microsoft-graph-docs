---
title: "Create plannerPlanDetails"
description: "Create a new plannerPlanDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create plannerPlanDetails

Namespace: microsoft.graph

Create a new [plannerPlanDetails](../resources/plannerplandetails.md) object.

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
POST ** Collection URI for microsoft.graph.plannerPlanDetails not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [plannerPlanDetails](../resources/plannerplandetails.md) object.

The following table shows the properties that are required when you create the [plannerPlanDetails](../resources/plannerplandetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)||
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)||



## Response
If successful, this method returns a `201 Created` response code and a [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannerplandetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.plannerPlanDetails not found
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerplandetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 510

{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "c44e8105-8105-c44e-0581-4ec405814ec4",
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

