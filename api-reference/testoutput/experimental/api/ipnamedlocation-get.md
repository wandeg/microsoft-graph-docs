---
title: "Get ipNamedLocation"
description: "Read properties and relationships of the ipNamedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get ipNamedLocation

Read properties and relationships of the [ipNamedLocation](../resources/ipnamedlocation.md) object.

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
GET ** Entity URI for microsoft.graph.ipNamedLocation not found
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
If successful, this method returns a `200 OK` response code and [ipNamedLocation](../resources/ipnamedlocation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_ipnamedlocation"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.ipNamedLocation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ipNamedLocation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 465

{
  "value": {
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
}
```

