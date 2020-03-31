---
title: "Get userAnalytics"
description: "Read properties and relationships of the userAnalytics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userAnalytics

Namespace: microsoft.graph

Read properties and relationships of the [userAnalytics](../resources/useranalytics.md) object.

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
GET /me/analytics
GET /users/{usersId}/analytics
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
If successful, this method returns a `200 OK` response code and [userAnalytics](../resources/useranalytics.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_useranalytics"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/analytics
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAnalytics"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "value": {
    "@odata.type": "#microsoft.graph.userAnalytics",
    "id": "86e55e79-5e79-86e5-795e-e586795ee586",
    "settings": {
      "@odata.type": "microsoft.graph.settings",
      "hasLicense": true,
      "hasOptedOut": true,
      "hasGraphMailbox": true
    }
  }
}
```

