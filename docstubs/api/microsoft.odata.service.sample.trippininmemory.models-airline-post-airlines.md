---
title: "Create Airline"
description: "Create a new Airline object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create Airline

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create a new [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.

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
POST /Airlines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.

The following table shows the properties that are required when you create the [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md).

|Property|Type|Description|
|:---|:---|:---|
|AirlineCode|String||
|Name|String||



## Response
If successful, this method returns a `201 Created` response code and a [Airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_airline_from_airlines"
}
-->
``` http
POST https://graph.microsoft.com/beta/Airlines
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airline",
  "AirlineCode": "Airline Code value",
  "Name": "Name value"
}
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
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 152

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.Airline",
  "AirlineCode": "Airline Code value",
  "Name": "Name value"
}
```

