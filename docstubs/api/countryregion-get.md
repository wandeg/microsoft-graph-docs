---
title: "Get countryRegion"
description: "Read properties and relationships of the countryRegion object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get countryRegion

Namespace: microsoft.graph

Read properties and relationships of the [countryRegion](../resources/countryregion.md) object.

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
GET /financials/companies/{companyId}/countriesRegions/{countryRegionId}
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
If successful, this method returns a `200 OK` response code and [countryRegion](../resources/countryregion.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_countryregion"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/countriesRegions/{countryRegionId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.countryRegion"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 308

{
  "value": {
    "@odata.type": "#microsoft.graph.countryRegion",
    "id": "45412536-2536-4541-3625-414536254145",
    "code": "Code value",
    "displayName": "Display Name value",
    "addressFormat": "Address Format value",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
  }
}
```

