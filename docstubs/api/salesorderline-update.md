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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salesorderline"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrderLines/{salesOrderLineId}
Content-type: application/json
Content-length: 926

{
  "@odata.type": "#microsoft.graph.salesOrderLine",
  "documentId": "2cd4c5df-c5df-2cd4-dfc5-d42cdfc5d42c",
  "sequence": 8,
  "itemId": "38e36916-6916-38e3-1669-e3381669e338",
  "accountId": "7085e644-e644-7085-44e6-857044e68570",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "af6b7225-7225-af6b-2572-6baf25726baf",
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
  "id": "f1758853-8853-f175-5388-75f1538875f1",
  "documentId": "2cd4c5df-c5df-2cd4-dfc5-d42cdfc5d42c",
  "sequence": 8,
  "itemId": "38e36916-6916-38e3-1669-e3381669e338",
  "accountId": "7085e644-e644-7085-44e6-857044e68570",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "af6b7225-7225-af6b-2572-6baf25726baf",
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

