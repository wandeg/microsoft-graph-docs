---
title: "Get officeGraphInsights"
description: "Read properties and relationships of an officeGraphInsights object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get officeGraphInsights

Namespace: microsoft.graph

Read properties and relationships of an [officeGraphInsights](../resources/officegraphinsights.md) object.

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
GET /me/insights
GET /users/{usersId}/insights
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
If successful, this method returns a `200 OK` response code and an [officeGraphInsights](../resources/officegraphinsights.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_officegraphinsights"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/insights
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officeGraphInsights"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.officeGraphInsights",
    "id": "53b952bc-52bc-53b9-bc52-b953bc52b953"
  }
}
```

