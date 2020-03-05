---
title: "List administrativeUnits"
description: "List properties and relationships of the administrativeUnit objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List administrativeUnits

Namespace: microsoft.graph

List properties and relationships of the [administrativeUnit](../resources/administrativeunit.md) objects.

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
GET ** Collection URI for microsoft.graph.administrativeUnit not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.administrativeUnit not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.administrativeunit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 213

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.administrativeUnit",
      "id": "e9ca2e59-2e59-e9ca-592e-cae9592ecae9",
      "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00"
    }
  ]
}
```

