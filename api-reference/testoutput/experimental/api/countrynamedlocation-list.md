---
title: "List countryNamedLocations"
description: "List properties and relationships of the countryNamedLocation objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List countryNamedLocations

List properties and relationships of the [countryNamedLocation](../resources/countrynamedlocation.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET ** Collection URI for microsoft.graph.countryNamedLocation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [countryNamedLocation](../resources/countrynamedlocation.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.countryNamedLocation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.countrynamedlocation)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 454

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.countryNamedLocation",
      "id": "859b3ee6-3ee6-859b-e63e-9b85e63e9b85",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
      "modifiedDateTime": "2017-01-01T00:03:12.7204145+03:00",
      "countriesAndRegions": [
        "Countries And Regions value"
      ],
      "includeUnknownCountriesAndRegions": true
    }
  ]
}
```

