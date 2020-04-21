---
title: "Create buckets"
description: "Create a new buckets object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create buckets

Namespace: microsoft.graph

Create a new buckets object.

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
POST /planner/buckets
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [plannerBucket](../resources/plannerbucket.md) object.

The following table shows the properties that are required when you create the [plannerBucket](../resources/plannerbucket.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|
|orderHint|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [plannerBucket](../resources/plannerbucket.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerbucket_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/planner/buckets
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerbucket"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "87713787-3787-8771-8737-718787377187",
  "name": "Name value",
  "planId": "Plan Id value",
  "orderHint": "Order Hint value"
}
```

