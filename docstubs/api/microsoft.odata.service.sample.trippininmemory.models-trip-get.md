---
title: "Get Trip"
description: "Read properties and relationships of the Trip object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get Trip

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Read properties and relationships of the [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.

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
If successful, this method returns a `200 OK` response code and [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_trip"
}
-->
``` http

```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.Trip"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 421

{
  "value": {
    "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Trip",
    "TripId": 6,
    "ShareId": "9f0bcd42-cd42-9f0b-42cd-0b9f42cd0b9f",
    "Name": "Name value",
    "Budget": "Single",
    "Description": "Description value",
    "Tags": [
      "Tags value"
    ],
    "StartsAt": "2017-01-01T00:01:10.6216491+03:00",
    "EndsAt": "2017-01-01T00:02:07.8652631+03:00"
  }
}
```

