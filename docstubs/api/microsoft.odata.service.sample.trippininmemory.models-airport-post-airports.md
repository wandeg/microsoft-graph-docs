---
title: "Create airport"
description: "Create a new airport object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create airport

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create a new [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.

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
POST /airports
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object.

The following table shows the properties that are required when you create the [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md).

|Property|Type|Description|
|:---|:---|:---|
|icaoCode|String||
|name|String||
|iataCode|String||
|location|[airportLocation](../resources/microsoft.odata.service.sample.trippininmemory.models-airportlocation.md)||



## Response
If successful, this method returns a `201 Created` response code and a [airport](../resources/microsoft.odata.service.sample.trippininmemory.models-airport.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_airport_from_airports"
}
-->
``` http
POST https://graph.microsoft.com/beta/airports
Content-type: application/json
Content-length: 545

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airport",
  "icaoCode": "Icao Code value",
  "name": "Name value",
  "iataCode": "Iata Code value",
  "location": {
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.odata.service.sample.trippininmemory.models.airport"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 545

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airport",
  "icaoCode": "Icao Code value",
  "name": "Name value",
  "iataCode": "Iata Code value",
  "location": {
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

