---
title: "Get salesOrderLine"
description: "Read properties and relationships of the salesOrderLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesOrderLine

Read properties and relationships of the [salesOrderLine](../resources/salesorderline.md) object.

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
GET /financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [salesOrderLine](../resources/salesorderline.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salesorderline"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
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
    "id": "44a90d72-0d72-44a9-720d-a944720da944",
    "documentId": "419d5728-5728-419d-2857-9d4128579d41",
    "sequence": 8,
    "itemId": "28a289c5-89c5-28a2-c589-a228c589a228",
    "accountId": "7538836d-836d-7538-6d83-38756d833875",
    "lineType": "Line Type value",
    "description": "Description value",
    "unitOfMeasureId": "9d7dd2ef-d2ef-9d7d-efd2-7d9defd27d9d",
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

