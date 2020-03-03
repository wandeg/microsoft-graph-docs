---
title: "Update ipNamedLocation"
description: "Update the properties of a ipNamedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update ipNamedLocation

Namespace: microsoft.graph

Update the properties of a [ipNamedLocation](../resources/ipnamedlocation.md) object.

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
PATCH ** Entity URI for microsoft.graph.ipNamedLocation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [ipNamedLocation](../resources/ipnamedlocation.md) object.

The following table shows the properties that are required when you create the [ipNamedLocation](../resources/ipnamedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [namedLocation](../resources/namedlocation.md)|
|createdDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedlocation.md)|
|modifiedDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedlocation.md)|
|ipRanges|[ipRange](../resources/iprange.md) collection||
|isTrusted|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_ipnamedlocation"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.ipNamedLocation not found
Content-type: application/json
Content-length: 254

{
  "@odata.type": "#microsoft.graph.ipNamedLocation",
  "displayName": "Display Name value",
  "ipRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange",
      "cidrAddress": "Cidr Address value"
    }
  ],
  "isTrusted": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 421

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
```

