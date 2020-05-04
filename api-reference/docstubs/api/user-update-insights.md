---
title: "Update insights"
description: "Update the properties of an insights object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update insights

Namespace: microsoft.graph

Update the properties of an insights object.

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
PATCH /me/insights
PATCH /users/{usersId}/insights
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [officeGraphInsights](../resources/officegraphinsights.md) object.

The following table shows the properties that are required when you create the [officeGraphInsights](../resources/officegraphinsights.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [officeGraphInsights](../resources/officegraphinsights.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_insights"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/insights
Content-Type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.officeGraphInsights"
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
  "@odata.type": "#microsoft.graph.officeGraphInsights",
  "id": "5e73abcc-abcc-5e73-ccab-735eccab735e"
}
```

