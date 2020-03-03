---
title: "Get payloadResponse"
description: "Read properties and relationships of the payloadResponse object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get payloadResponse

Namespace: microsoft.graph

Read properties and relationships of the [payloadResponse](../resources/payloadresponse.md) object.

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
GET /payloadResponse/{payloadResponseId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [payloadResponse](../resources/payloadresponse.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_payloadresponse"
}
-->
``` http
GET https://graph.microsoft.com/localtest/payloadResponse/{payloadResponseId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.payloadResponse"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 129

{
  "value": {
    "@odata.type": "#microsoft.graph.payloadResponse",
    "id": "425e067d-067d-425e-7d06-5e427d065e42"
  }
}
```

