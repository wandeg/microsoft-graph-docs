---
title: "Update Airport"
description: "Update the properties of a Airport object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update Airport

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.

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
PATCH /Airports/{AirportsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.

The following table shows the properties that are required when you create the [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md).

|Property|Type|Description|
|:---|:---|:---|
|IcaoCode|String||
|Name|String||
|IataCode|String||
|Location|[AirportLocation](../resources/microsoft.odata.service.sample.trippininmemory.models-airportlocation.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [Airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_airport"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/Airports/{AirportsId}
Content-type: application/json
Content-length: 545

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airport",
  "IcaoCode": "Icao Code value",
  "Name": "Name value",
  "IataCode": "Iata Code value",
  "Location": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.AirportLocation",
    "Address": "Address value",
    "City": {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
      "CountryRegion": "Country Region value",
      "Region": "Region value"
    },
    "Loc": "GeographyPoint"
  }
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
Content-Length: 545

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airport",
  "IcaoCode": "Icao Code value",
  "Name": "Name value",
  "IataCode": "Iata Code value",
  "Location": {
    "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.AirportLocation",
    "Address": "Address value",
    "City": {
      "@odata.type": "Microsoft.OData.Service.Sample.TrippinInMemory.Models.City",
      "CountryRegion": "Country Region value",
      "Region": "Region value"
    },
    "Loc": "GeographyPoint"
  }
}
```

