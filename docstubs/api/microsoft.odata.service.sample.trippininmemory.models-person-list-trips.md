---
title: "List trips"
description: "Get the trips from the trips navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List trips

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Get the trips from the trips navigation property.

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
GET /me/trips
GET /people/{peopleId}/trips
GET /newComePeople/{newComePeopleId}/trips
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
If successful, this method returns a `200 OK` response code and a collection of [trip](../resources/trip.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_trip"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/trips
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.odata.service.sample.trippininmemory.models.trip)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 457

{
  "value": [
    {
      "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.trip",
      "tripId": 6,
      "shareId": "730a3275-3275-730a-7532-0a7375320a73",
      "name": "Name value",
      "budget": "Single",
      "description": "Description value",
      "tags": [
        "Tags value"
      ],
      "startsAt": "2016-12-31T23:56:46.9049138+03:00",
      "endsAt": "2016-12-31T23:57:07.6482324+03:00"
    }
  ]
}
```

