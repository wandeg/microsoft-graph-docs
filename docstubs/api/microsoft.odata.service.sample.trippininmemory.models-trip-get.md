---
title: "Get trip"
description: "Read properties and relationships of the trip object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get trip

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Read properties and relationships of the [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.

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
If successful, this method returns a `200 OK` response code and [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_trip"
}
-->
``` http

```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.trip"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 429

{
  "value": {
    "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.trip",
    "tripId": 6,
    "shareId": "c2f105cb-05cb-c2f1-cb05-f1c2cb05f1c2",
    "name": "Name value",
    "budget": "Single",
    "description": "Description value",
    "tags": [
      "Tags value"
    ],
    "startsAtDateTime": "2017-01-01T00:02:51.9468808+03:00",
    "endsAt": "2016-12-31T23:58:09.1044492+03:00"
  }
}
```

