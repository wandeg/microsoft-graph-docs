---
title: "List salesOrderLines"
description: "Get the salesOrderLines from the salesOrderLines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesOrderLines

Namespace: microsoft.graph

Get the salesOrderLines from the salesOrderLines navigation property.

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
GET /financials/companies/{companyId}/salesOrderLines
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
If successful, this method returns a `200 OK` response code and a collection of [salesOrderLine](../resources/salesorderline.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesorderline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrderLines
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesorderline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1120

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesOrderLine",
      "id": "fffc44ee-44ee-fffc-ee44-fcffee44fcff",
      "documentId": "05b0fe26-fe26-05b0-26fe-b00526feb005",
      "sequence": 8,
      "itemId": "cbb5810f-810f-cbb5-0f81-b5cb0f81b5cb",
      "accountId": "7c4a388a-388a-7c4a-8a38-4a7c8a384a7c",
      "lineType": "Line Type value",
      "description": "Description value",
      "unitOfMeasureId": "7bdb3368-3368-7bdb-6833-db7b6833db7b",
      "quantity": "4.2",
      "unitPrice": "4.2",
      "discountAmount": "4.2",
      "discountPercent": "4.2",
      "discountAppliedBeforeTax": true,
      "amountExcludingTax": "4.2",
      "taxCode": "Tax Code value",
      "taxPercent": "4.2",
      "totalTaxAmount": "4.2",
      "amountIncludingTax": "4.2",
      "invoiceDiscountAllocation": "4.2",
      "netAmount": "4.2",
      "netTaxAmount": "4.2",
      "netAmountIncludingTax": "4.2",
      "shipmentDate": "Date",
      "shippedQuantity": "4.2",
      "invoicedQuantity": "4.2",
      "invoiceQuantity": "4.2",
      "shipQuantity": "4.2"
    }
  ]
}
```

