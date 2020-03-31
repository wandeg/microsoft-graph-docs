---
title: "Get salesOrderLine"
description: "Read properties and relationships of the salesOrderLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesOrderLine

Namespace: microsoft.graph

Read properties and relationships of the [salesOrderLine](../resources/salesorderline.md) object.

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
GET /financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}
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
If successful, this method returns a `200 OK` response code and [salesOrderLine](../resources/salesorderline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesorderline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesOrderLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1050

{
  "value": {
    "@odata.type": "#microsoft.graph.salesOrderLine",
    "id": "d25f7582-7582-d25f-8275-5fd282755fd2",
    "documentId": "a96669d7-69d7-a966-d769-66a9d76966a9",
    "sequence": 8,
    "itemId": "aefdf05f-f05f-aefd-5ff0-fdae5ff0fdae",
    "accountId": "ecadd616-d616-ecad-16d6-adec16d6adec",
    "lineType": "Line Type value",
    "description": "Description value",
    "unitOfMeasureId": "9f28e186-e186-9f28-86e1-289f86e1289f",
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
}
```

