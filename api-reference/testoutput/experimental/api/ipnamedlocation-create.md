---
title: "Create ipNamedLocation"
description: "Create a new ipNamedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create ipNamedLocation

Create a new [ipNamedLocation](../resources/ipnamedlocation.md) object.

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
POST ** Collection URI for microsoft.graph.ipNamedLocation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the ipNamedLocation object.

The following table shows the properties that are required when you create the ipNamedLocation.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [namedLocation](../resources/namedLocation.md)|
|createdDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|
|modifiedDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|
|ipRanges|[ipRange](../resources/ipRange.md) collection||
|isTrusted|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_ipnamedlocation_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.ipNamedLocation not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.ipnamedlocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 422

{
  "@odata.type": "#microsoft.graph.ipNamedLocation",
  "id": "9cf593ef-93ef-9cf5-ef93-f59cef93f59c",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "modifiedDateTime": "2017-01-01T00:03:12.7204145+03:00",
  "ipRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange",
      "cidrAddress": "Cidr Address value"
    }
  ],
  "isTrusted": true
}
```

