---
title: "List privilegedAccesses"
description: "List properties and relationships of the privilegedAccess objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List privilegedAccesses

Namespace: microsoft.graph

List properties and relationships of the [privilegedAccess](../resources/privilegedaccess.md) objects.

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
GET /privilegedAccess
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [privilegedAccess](../resources/privilegedaccess.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedaccess"
}
-->
``` http
GET https://graph.microsoft.com/localtest/privilegedAccess
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.privilegedaccess)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 192

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.privilegedAccess",
      "id": "0d80c281-c281-0d80-81c2-800d81c2800d",
      "displayName": "Display Name value"
    }
  ]
}
```

