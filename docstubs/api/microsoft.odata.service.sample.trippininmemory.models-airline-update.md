---
title: "Update airline"
description: "Update the properties of a airline object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update airline

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Update the properties of a [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.

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
PATCH /airlines/{airlinesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object.

The following table shows the properties that are required when you create the [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md).

|Property|Type|Description|
|:---|:---|:---|
|airlineCode|String||
|name|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [airline](../resources/microsoft.odata.service.sample.trippininmemory.models-airline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_airline"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/airlines/{airlinesId}
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airline",
  "airlineCode": "Airline Code value",
  "name": "Name value"
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
Content-Length: 152

{
  "@odata.type": "#Microsoft.OData.Service.Sample.TrippinInMemory.Models.airline",
  "airlineCode": "Airline Code value",
  "name": "Name value"
}
```

