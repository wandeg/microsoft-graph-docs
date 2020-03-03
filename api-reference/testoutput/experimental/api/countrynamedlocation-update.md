---
title: "Update countryNamedLocation"
description: "Update the properties of a countryNamedLocation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update countryNamedLocation

Update the properties of a [countryNamedLocation](../resources/countrynamedlocation.md) object.

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
PATCH ** Entity URI for microsoft.graph.countryNamedLocation not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [countryNamedLocation](../resources/countryNamedLocation.md) object.

The following table shows the properties that are required when you create the [countryNamedLocation](../resources/countrynamedlocation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|displayName|String| Inherited from [namedLocation](../resources/namedLocation.md)|
|createdDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|
|modifiedDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|
|countriesAndRegions|String collection||
|includeUnknownCountriesAndRegions|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [countryNamedLocation](../resources/countrynamedlocation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_countrynamedlocation"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.countryNamedLocation not found
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

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
```

