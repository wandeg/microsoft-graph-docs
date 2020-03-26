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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privilegedAccess
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
If successful, this method returns a `200 OK` response code and a collection of [privilegedAccess](../resources/privilegedaccess.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_privilegedaccess"
}
-->
``` http
GET https://graph.microsoft.com/beta/privilegedAccess
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
      "id": "015a5f24-5f24-015a-245f-5a01245f5a01",
      "displayName": "Display Name value"
    }
  ]
}
```

