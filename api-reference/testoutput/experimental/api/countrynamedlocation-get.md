---
title: "Get countryNamedLocation"
description: "Read properties and relationships of the countryNamedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get countryNamedLocation

Namespace: microsoft.graph

Read properties and relationships of the [countryNamedLocation](../resources/countrynamedlocation.md) object.

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
GET ** Entity URI for microsoft.graph.countryNamedLocation not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_countrynamedlocation"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.countryNamedLocation not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryNamedLocation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 421

{
  "value": {
    "@odata.type": "#microsoft.graph.countryNamedLocation",
    "id": "29756ff1-6ff1-2975-f16f-7529f16f7529",
    "displayName": "Display Name value",
    "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
    "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
    "countriesAndRegions": [
      "Countries And Regions value"
    ],
    "includeUnknownCountriesAndRegions": true
  }
}
```

