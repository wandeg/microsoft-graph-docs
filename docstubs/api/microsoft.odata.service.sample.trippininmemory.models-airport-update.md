---
title: "Update airport"
description: "Update the properties of a airport object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update airport

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.

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
PATCH /airports/{airportsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.

The following table shows the properties that are required when you create the [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md).

|Property|Type|Description|
|:---|:---|:---|
|icaoCode|String||
|name|String||
|iataCode|String||
|airpLocation|[airportLocation](../resources/microsoft.odata.service.sample.trippininmemory.models-airportlocation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_airport"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/airports/{airportsId}
Content-type: application/json
Content-length: 549

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airport",
  "icaoCode": "Icao Code value",
  "name": "Name value",
  "iataCode": "Iata Code value",
  "airpLocation": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.airportLocation",
    "address": "Address value",
    "city": {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
      "countryRegion": "Country Region value",
      "region": "Region value"
    },
    "loc": "GeographyPoint"
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 549

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airport",
  "icaoCode": "Icao Code value",
  "name": "Name value",
  "iataCode": "Iata Code value",
  "airpLocation": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.airportLocation",
    "address": "Address value",
    "city": {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.city",
      "countryRegion": "Country Region value",
      "region": "Region value"
    },
    "loc": "GeographyPoint"
  }
}
```

