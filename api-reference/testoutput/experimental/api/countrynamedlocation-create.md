---
title: "Create countryNamedLocation"
description: "Create a new countryNamedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create countryNamedLocation

Namespace: microsoft.graph

Create a new [countryNamedLocation](../resources/countrynamedlocation.md) object.

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
POST ** Collection URI for microsoft.graph.countryNamedLocation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [countryNamedLocation](../resources/countrynamedlocation.md) object.

The following table shows the properties that are required when you create the [countryNamedLocation](../resources/countrynamedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [namedLocation](../resources/namedlocation.md)|
|createdDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedlocation.md)|
|modifiedDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedlocation.md)|
|countriesAndRegions|String collection||
|includeUnknownCountriesAndRegions|Boolean||



## Response
If successful, this method returns a `201 Created` response code and a [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_countrynamedlocation_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.countryNamedLocation not found
Content-type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.countryNamedLocation",
  "displayName": "Display Name value",
  "countriesAndRegions": [
    "Countries And Regions value"
  ],
  "includeUnknownCountriesAndRegions": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countrynamedlocation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 384

{
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
```

