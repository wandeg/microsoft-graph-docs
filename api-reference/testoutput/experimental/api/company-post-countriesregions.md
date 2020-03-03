---
title: "Add countriesRegions"
description: "Add countriesRegions by posting to the countriesRegions collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add countriesRegions

Add countriesRegions by posting to the countriesRegions collection.

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
POST /financials/companies/{companyId}/countriesRegions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the countryRegion object.

The following table shows the properties that are required when you create the countryRegion.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|addressFormat|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [countryRegion](../resources/countryregion.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_countryregion_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/financials/companies/{companyId}/countriesRegions
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
  "truncated": true,
  "@odata.type": "microsoft.graph.countryregion"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 277

{
  "@odata.type": "#microsoft.graph.countryRegion",
  "id": "2172a90e-a90e-2172-0ea9-72210ea97221",
  "code": "Code value",
  "displayName": "Display Name value",
  "addressFormat": "Address Format value",
  "lastModifiedDateTime": "2016-12-31T23:58:46.8102575+03:00"
}
```

