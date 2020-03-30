---
title: "Update countryRegion"
description: "Update the properties of a countryRegion object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update countryRegion

Namespace: microsoft.graph

Update the properties of a [countryRegion](../resources/countryregion.md) object.

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
PATCH /financials/companies/{companyId}/countriesRegions/{countryRegionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [countryRegion](../resources/countryregion.md) object.

The following table shows the properties that are required when you create the [countryRegion](../resources/countryregion.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|addressFormat|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [countryRegion](../resources/countryregion.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_countryregion"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/countriesRegions/{countryRegionId}
Content-type: application/json
Content-length: 164

{
  "@odata.type": "#microsoft.graph.countryRegion",
  "code": "Code value",
  "displayName": "Display Name value",
  "addressFormat": "Address Format value"
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
Content-Length: 277

{
  "@odata.type": "#microsoft.graph.countryRegion",
  "id": "e4141b41-1b41-e414-411b-14e4411b14e4",
  "code": "Code value",
  "displayName": "Display Name value",
  "addressFormat": "Address Format value",
  "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00"
}
```

