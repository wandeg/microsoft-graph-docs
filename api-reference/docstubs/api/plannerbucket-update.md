---
title: "Update plannerBucket"
description: "Update the properties of a plannerBucket object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update plannerBucket

Namespace: microsoft.graph

Update the properties of a [plannerBucket](../resources/plannerbucket.md) object.

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
PATCH /planner/buckets/{plannerBucketId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [plannerBucket](../resources/plannerbucket.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_plannerbucket"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/planner/buckets/{plannerBucketId}
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerBucket",
  "id": "87713787-3787-8771-8737-718787377187",
  "name": "Name value",
  "planId": "Plan Id value",
  "orderHint": "Order Hint value"
}
```

