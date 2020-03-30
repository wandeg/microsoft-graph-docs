---
title: "List governanceResources"
description: "List properties and relationships of the governanceResource objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List governanceResources

Namespace: microsoft.graph

List properties and relationships of the [governanceResource](../resources/governanceresource.md) objects.

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
GET /governanceResources
GET /privilegedAccess/{privilegedAccessId}/resources
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
If successful, this method returns a `200 OK` response code and a collection of [governanceResource](../resources/governanceresource.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/governanceResources
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.governanceresource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.governanceResource",
      "id": "bc1e25c6-25c6-bc1e-c625-1ebcc6251ebc",
      "externalId": "External Id value",
      "type": "Type value",
      "displayName": "Display Name value",
      "status": "Status value",
      "registeredDateTime": "2017-01-01T00:00:37.1297883+03:00",
      "registeredRoot": "Registered Root value"
    }
  ]
}
```

