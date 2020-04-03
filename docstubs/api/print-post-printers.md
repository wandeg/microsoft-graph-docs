---
title: "Add printers"
description: "Add printers by posting to the printers collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add printers

Namespace: microsoft.graph

Add printers by posting to the printers collection.

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
POST /print/printers/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [printer](../resources/printer.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_printer_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/print/printers
Content-type: application/json
Content-length: 1817

{
  "@odata.type": "#microsoft.graph.printer",
  "name": "Name value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "registeredDateTime": "2017-01-01T00:02:54.6216401+00:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1866

{
  "@odata.type": "#microsoft.graph.printer",
  "id": "91523cd4-3cd4-9152-d43c-5291d43c5291",
  "name": "Name value",
  "manufacturer": "Manufacturer value",
  "model": "Model value",
  "registeredDateTime": "2017-01-01T00:02:54.6216401+00:00",
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

