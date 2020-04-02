---
title: "GetFavoriteAirline"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# GetFavoriteAirline

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models



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
GET /Me/GetFavoriteAirline
GET /People/{PeopleId}/GetFavoriteAirline
GET /NewComePeople/{NewComePeopleId}/GetFavoriteAirline
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "person_getfavoriteairline"
}
-->
``` http
GET https://graph.microsoft.com/beta/Me/GetFavoriteAirline
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.odata.service.sample.trippininmemory.models.airline"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 177

{
  "value": {
    "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airline",
    "AirlineCode": "Airline Code value",
    "Name": "Name value"
  }
}
```

