---
title: "List paymentMethod"
description: "Get the paymentMethods from the paymentMethod navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List paymentMethod

Namespace: microsoft.graph

Get the paymentMethods from the paymentMethod navigation property.

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
GET /financials/companies/{companyId}/vendors/{vendorId}/paymentMethod
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [paymentMethod](../resources/paymentmethod.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_paymentmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors/{vendorId}/paymentMethod
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.paymentmethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.paymentMethod",
      "id": "d1d31e7b-1e7b-d1d3-7b1e-d3d17b1ed3d1",
      "code": "String",
      "displayName": "String",
      "lastModifiedDateTime": "String (timestamp)"
    }
  ]
}
```

