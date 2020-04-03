---
title: "Add connectors"
description: "Add connectors by posting to the connectors collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add connectors

Namespace: microsoft.graph

Add connectors by posting to the connectors collection.

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
POST /print/connectors/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [printConnector](../resources/printconnector.md) object.

The following table shows the properties that are required when you create the [printConnector](../resources/printconnector.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|fullyQualifiedDomainName|String||
|operatingSystem|String||
|appVersion|String||
|deviceHealth|[deviceHealth](../resources/devicehealth.md)||
|location|[printerLocation](../resources/printerlocation.md)||
|registeredDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [printConnector](../resources/printconnector.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printconnector_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/connectors
Content-type: application/json
Content-length: 1190

{
  "@odata.type": "#microsoft.graph.printConnector",
  "name": "Name value",
  "fullyQualifiedDomainName": "Fully Qualified Domain Name value",
  "operatingSystem": "Operating System value",
  "appVersion": "App Version value",
  "deviceHealth": {
    "@odata.type": "microsoft.graph.deviceHealth",
    "lastConnectionTime": "2017-01-01T00:02:32.6478319+00:00"
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
  "registeredDateTime": "2017-01-01T00:02:54.6216401+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printconnector"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1239

{
  "@odata.type": "#microsoft.graph.printConnector",
  "id": "f5ae8e9c-8e9c-f5ae-9c8e-aef59c8eaef5",
  "name": "Name value",
  "fullyQualifiedDomainName": "Fully Qualified Domain Name value",
  "operatingSystem": "Operating System value",
  "appVersion": "App Version value",
  "deviceHealth": {
    "@odata.type": "microsoft.graph.deviceHealth",
    "lastConnectionTime": "2017-01-01T00:02:32.6478319+00:00"
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
  "registeredDateTime": "2017-01-01T00:02:54.6216401+00:00"
}
```

