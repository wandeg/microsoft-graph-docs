---
title: "List dimensionValues"
description: "Get the dimensionValues from the dimensionValues navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List dimensionValues

Namespace: microsoft.graph

Get the dimensionValues from the dimensionValues navigation property.

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
GET /financials/companies/{companyId}/dimensions/{dimensionId}/dimensionValues
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
If successful, this method returns a `200 OK` response code and a collection of [dimensionValue](../resources/dimensionvalue.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_dimensionvalue"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/dimensions/{dimensionId}/dimensionValues
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.dimensionvalue)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dimensionValue",
      "id": "9382060c-060c-9382-0c06-82930c068293",
      "code": "Code value",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
    }
  ]
}
```

