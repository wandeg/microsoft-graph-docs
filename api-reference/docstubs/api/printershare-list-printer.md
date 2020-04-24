---
title: "List printer"
description: "Get the printers from the printer navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List printer

Namespace: microsoft.graph

Get the printers from the printer navigation property.

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
GET /print/printers/{printerId}/share/printer
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
If successful, this method returns a `200 OK` response code and a collection of [printer](../resources/printer.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printer"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/share/printer
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.printer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.printer",
      "id": "525447d8-47d8-5254-d847-5452d8475452",
      "name": "Name value",
      "manufacturer": "Manufacturer value",
      "model": "Model value",
      "registeredDateTime": "2017-01-01T00:00:25.9110048+03:00",
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
  ]
}
```

