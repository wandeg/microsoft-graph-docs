---
title: "List connectors"
description: "Get the printConnectors from the connectors navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List connectors

Namespace: microsoft.graph

Get the printConnectors from the connectors navigation property.

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
GET /print/printers/{printerId}/connectors
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
If successful, this method returns a `200 OK` response code and a collection of [printConnector](../resources/printconnector.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_printconnector"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/connectors
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printconnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1420

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printConnector",
      "id": "75677838-7838-7567-3878-677538786775",
      "name": "Name value",
      "fullyQualifiedDomainName": "Fully Qualified Domain Name value",
      "operatingSystem": "Operating System value",
      "appVersion": "App Version value",
      "deviceHealth": {
        "@odata.type": "microsoft.graph.deviceHealth",
        "lastConnectionTime": "2016-12-31T23:57:15.2770821+00:00"
      },
      "location": {
        "@odata.type": "microsoft.graph.printerLocation",
        "latitude": "Single",
        "longitude": "Single",
        "altitudeInMeters": 0,
        "streetAddress": "Street Address value",
        "subunit": [
          "Subunit value"
        ],
        "city": "City value",
        "postalCode": "Postal Code value",
        "countryOrRegion": "Country Or Region value",
        "site": "Site value",
        "building": "Building value",
        "floorNumber": 11,
        "floorDescription": "Floor Description value",
        "roomNumber": 10,
        "roomDescription": "Room Description value",
        "organization": [
          "Organization value"
        ],
        "subdivision": [
          "Subdivision value"
        ],
        "stateOrProvince": "State Or Province value"
      },
      "registeredDateTime": "2016-12-31T23:56:45.5677434+00:00"
    }
  ]
}
```

