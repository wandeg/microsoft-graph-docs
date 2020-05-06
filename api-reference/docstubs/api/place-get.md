---
title: "Get place"
description: "Read properties and relationships of a place object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get place

Namespace: microsoft.graph

Read properties and relationships of a [place](../resources/place.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /places/{placesId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [place](../resources/place.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_place"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/places/{placesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.place"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.place",
    "id": "f758c435-c435-f758-35c4-58f735c458f7",
    "displayName": "Display Name value",
    "geoCoordinates": {
      "@odata.type": "microsoft.graph.outlookGeoCoordinates",
      "latitude": "Double",
      "longitude": "Double",
      "accuracy": "Double",
      "altitude": "Double",
      "altitudeAccuracy": "Double"
    },
    "phone": "Phone value",
    "address": {
      "@odata.type": "microsoft.graph.physicalAddress",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryOrRegion": "Country Or Region value",
      "postalCode": "Postal Code value"
    }
  }
}
```

