---
title: "Create trips"
description: "Create trips by posting to the trips collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create trips

Namespace: Microsoft.OData.Service.Sample.TrippinInMemory.Models

Create trips by posting to the trips collection.

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
POST /me/trips/$ref
POST /people/{peopleId}/trips/$ref
POST /newComePeople/{newComePeopleId}/trips/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object.

The following table shows the properties that are required when you create the [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md).

|Property|Type|Description|
|:---|:---|:---|
|tripId|Int32||
|shareId|Guid||
|name|String||
|budget|Single||
|description|String||
|tags|String collection||
|startsAtDateTime|DateTimeOffset||
|endsAt|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [trip](../resources/microsoft.odata.service.sample.trippininmemory.models-trip.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_trip_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/trips
Content-type: application/json
Content-length: 388

{
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.odata.service.sample.trippininmemory.models.trip"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 388

{
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
```

