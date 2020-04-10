---
title: "Get taxArea"
description: "Read properties and relationships of the taxArea object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get taxArea

Namespace: microsoft.graph

Read properties and relationships of the [taxArea](../resources/taxarea.md) object.

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
GET /financials/companies/{companyId}/taxAreas/{taxAreaId}
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
If successful, this method returns a `200 OK` response code and [taxArea](../resources/taxarea.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_taxarea"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/taxAreas/{taxAreaId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taxArea"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 290

{
  "value": {
    "@odata.type": "#microsoft.graph.taxArea",
    "id": "f42cbd2c-bd2c-f42c-2cbd-2cf42cbd2cf4",
    "code": "Code value",
    "displayName": "Display Name value",
    "taxType": "Tax Type value",
    "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
  }
}
```

