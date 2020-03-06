---
title: "Get informationProtection"
description: "Read properties and relationships of the informationProtection object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get informationProtection

Namespace: microsoft.graph

Read properties and relationships of the [informationProtection](../resources/informationprotection.md) object.

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
GET /informationProtection
GET /me/informationProtection
GET /users/{usersId}/informationProtection
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [informationProtection](../resources/informationprotection.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_informationprotection"
}
-->
``` http
GET https://graph.microsoft.com/localtest/informationProtection
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.informationProtection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 135

{
  "value": {
    "@odata.type": "#microsoft.graph.informationProtection",
    "id": "f859873c-873c-f859-3c87-59f83c8759f8"
  }
}
```

