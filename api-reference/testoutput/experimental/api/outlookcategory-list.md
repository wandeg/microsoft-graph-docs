---
title: "List outlookCategories"
description: "List properties and relationships of the outlookCategory objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List outlookCategories

Namespace: microsoft.graph

List properties and relationships of the [outlookCategory](../resources/outlookcategory.md) objects.

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
GET /me/outlook/masterCategories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [outlookCategory](../resources/outlookcategory.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_outlookcategory"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/outlook/masterCategories
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.outlookcategory)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 217

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.outlookCategory",
      "id": "a1e7cb3b-cb3b-a1e7-3bcb-e7a13bcbe7a1",
      "displayName": "Display Name value",
      "color": "String"
    }
  ]
}
```

