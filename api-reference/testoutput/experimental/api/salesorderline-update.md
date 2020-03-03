---
title: "Update salesOrderLine"
description: "Update the properties of a salesOrderLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesOrderLine

Namespace: microsoft.graph

Update the properties of a [salesOrderLine](../resources/salesorderline.md) object.

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
PATCH /financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [salesOrderLine](../resources/salesorderline.md) object.

The following table shows the properties that are required when you create the [salesOrderLine](../resources/salesorderline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|documentId|Guid||
|sequence|Int32||
|itemId|Guid||
|accountId|Guid||
|lineType|String||
|description|String||
|unitOfMeasureId|Guid||
|quantity|Decimal||
|unitPrice|Decimal||
|discountAmount|Decimal||
|discountPercent|Decimal||
|discountAppliedBeforeTax|Boolean||
|amountExcludingTax|Decimal||
|taxCode|String||
|taxPercent|Decimal||
|totalTaxAmount|Decimal||
|amountIncludingTax|Decimal||
|invoiceDiscountAllocation|Decimal||
|netAmount|Decimal||
|netTaxAmount|Decimal||
|netAmountIncludingTax|Decimal||
|shipmentDate|Date||
|shippedQuantity|Decimal||
|invoicedQuantity|Decimal||
|invoiceQuantity|Decimal||
|shipQuantity|Decimal||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesOrderLine](../resources/salesorderline.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salesorderline"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
Content-type: application/json
Content-length: 926

{
  "@odata.type": "#microsoft.graph.salesOrderLine",
  "documentId": "a4d6f8da-f8da-a4d6-daf8-d6a4daf8d6a4",
  "sequence": 8,
  "itemId": "d76ea287-a287-d76e-87a2-6ed787a26ed7",
  "accountId": "95554513-4513-9555-1345-559513455595",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "c915dcf5-dcf5-c915-f5dc-15c9f5dc15c9",
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
Content-Length: 975

{
  "@odata.type": "#microsoft.graph.salesOrderLine",
  "id": "54b45e60-5e60-54b4-605e-b454605eb454",
  "documentId": "a4d6f8da-f8da-a4d6-daf8-d6a4daf8d6a4",
  "sequence": 8,
  "itemId": "d76ea287-a287-d76e-87a2-6ed787a26ed7",
  "accountId": "95554513-4513-9555-1345-559513455595",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "c915dcf5-dcf5-c915-f5dc-15c9f5dc15c9",
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
```

