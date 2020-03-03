---
title: "List ipNamedLocations"
description: "List properties and relationships of the ipNamedLocation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List ipNamedLocations

Namespace: microsoft.graph

List properties and relationships of the [ipNamedLocation](../resources/ipnamedlocation.md) objects.

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
GET ** Collection URI for microsoft.graph.ipNamedLocation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [ipNamedLocation](../resources/ipnamedlocation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.ipNamedLocation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.ipnamedlocation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 502

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ipNamedLocation",
      "id": "43c5943f-943f-43c5-3f94-c5433f94c543",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
      "ipRanges": [
        {
          "@odata.type": "microsoft.graph.iPv4CidrRange",
          "cidrAddress": "Cidr Address value"
        }
      ],
      "isTrusted": true
    }
  ]
}
```

