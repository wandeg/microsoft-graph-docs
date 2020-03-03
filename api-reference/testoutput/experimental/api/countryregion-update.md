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

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /financials/companies/{companyId}/countriesRegions/{countryRegionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

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

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_countryregion"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/countriesRegions/{countryRegionId}
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
  "id": "0c101412-1412-0c10-1214-100c1214100c",
  "code": "Code value",
  "displayName": "Display Name value",
  "addressFormat": "Address Format value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

