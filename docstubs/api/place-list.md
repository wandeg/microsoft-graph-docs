---
title: "List places"
description: "List properties and relationships of the place objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List places

Namespace: microsoft.graph

List properties and relationships of the [place](../resources/place.md) objects.

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
GET /places
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
If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_place"
}
-->
``` http
GET https://graph.microsoft.com/beta/places
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.place)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 841

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.place",
      "id": "f66395a0-95a0-f663-a095-63f6a09563f6",
      "displayName": "Display Name value",
      "geoCoordinates": {
        "@odata.type": "microsoft.graph.outlookGeoCoordinates",
        "altitude": "Double",
        "latitude": "Double",
        "longitude": "Double",
        "accuracy": "Double",
        "altitudeAccuracy": "Double"
      },
      "phone": "Phone value",
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress",
        "type": "String",
        "postOfficeBox": "Post Office Box value",
        "street": "Street value",
        "city": "City value",
        "state": "State value",
        "countryOrRegion": "Country Or Region value",
        "postalCode": "Postal Code value"
      }
    }
  ]
}
```

