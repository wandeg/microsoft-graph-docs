---
title: "Update printer"
description: "Update the properties of a printer object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update printer

Namespace: microsoft.graph

Update the properties of a [printer](../resources/printer.md) object.

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
PATCH /print/printers/{printerId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [printer](../resources/printer.md) object.

The following table shows the properties that are required when you create the [printer](../resources/printer.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|manufacturer|String||
|model|String||
|registeredDateTime|DateTimeOffset||
|status|[printerStatus](../resources/printerstatus.md)||
|isShared|Boolean||
|acceptingJobs|Boolean||
|location|[printerLocation](../resources/printerlocation.md)||
|defaults|[printerDefaults](../resources/printerdefaults.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_printer"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/print/printers/{printerId}
Content-type: application/json
Content-length: 1817

{
  "@odata.type": "#microsoft.graph.printer",
  "name": "Name value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "registeredDateTime": "2017-01-01T00:01:32.8610447+03:00",
  "status": {
    "@odata.type": "microsoft.graph.printerStatus",
    "processingState": "String",
    "processingStateReasons": [
      "String"
    ],
    "processingStateDescription": "Processing State Description value"
  },
  "isShared": true,
  "acceptingJobs": true,
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
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults",
    "copiesPerJob": 12,
    "documentMimeType": "Document Mime Type value",
    "finishings": [
      "String"
    ],
    "mediaColor": "Media Color value",
    "mediaType": "String",
    "mediaSize": "Media Size value",
    "pagesPerSheet": 13,
    "orientation": "String",
    "outputBin": "Output Bin value",
    "pdfFitToPage": true,
    "presentationDirection": "String",
    "printColorConfiguration": "String",
    "printQuality": "String",
    "duplexConfiguration": "String"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1866

{
  "@odata.type": "#microsoft.graph.printer",
  "id": "f3dbbb36-bb36-f3db-36bb-dbf336bbdbf3",
  "name": "Name value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "registeredDateTime": "2017-01-01T00:01:32.8610447+03:00",
  "status": {
    "@odata.type": "microsoft.graph.printerStatus",
    "processingState": "String",
    "processingStateReasons": [
      "String"
    ],
    "processingStateDescription": "Processing State Description value"
  },
  "isShared": true,
  "acceptingJobs": true,
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
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults",
    "copiesPerJob": 12,
    "documentMimeType": "Document Mime Type value",
    "finishings": [
      "String"
    ],
    "mediaColor": "Media Color value",
    "mediaType": "String",
    "mediaSize": "Media Size value",
    "pagesPerSheet": 13,
    "orientation": "String",
    "outputBin": "Output Bin value",
    "pdfFitToPage": true,
    "presentationDirection": "String",
    "printColorConfiguration": "String",
    "printQuality": "String",
    "duplexConfiguration": "String"
  }
}
```

