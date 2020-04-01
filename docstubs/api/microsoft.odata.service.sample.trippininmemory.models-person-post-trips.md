---
title: "Create Trips"
description: "Create Trips by posting to the Trips collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create Trips

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create Trips by posting to the Trips collection.

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
POST /Me/Trips/$ref
POST /People/{PeopleId}/Trips/$ref
POST /NewComePeople/{NewComePeopleId}/Trips/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.

The following table shows the properties that are required when you create the [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md).

|Property|Type|Description|
|:---|:---|:---|
|TripId|Int32||
|ShareId|Guid||
|Name|String||
|Budget|Single||
|Description|String||
|Tags|String collection||
|StartsAt|DateTimeOffset||
|EndsAt|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [Trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_trip_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/Me/Trips
Content-type: application/json
Content-length: 380

{
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.odata.service.sample.trippininmemory.models.trip"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 380

{
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
```

