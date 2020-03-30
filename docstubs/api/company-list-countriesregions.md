---
title: "List countriesRegions"
description: "Get the countryRegions from the countriesRegions navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List countriesRegions

Namespace: microsoft.graph

Get the countryRegions from the countriesRegions navigation property.

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
GET /financials/companies/{companyId}/countriesRegions
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
If successful, this method returns a `200 OK` response code and a collection of [countryRegion](../resources/countryregion.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_countryregion"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/countriesRegions
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.countryregion)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 334

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.countryRegion",
      "id": "1516f44a-f44a-1516-4af4-16154af41615",
      "code": "Code value",
      "displayName": "Display Name value",
      "addressFormat": "Address Format value",
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00"
    }
  ]
}
```

