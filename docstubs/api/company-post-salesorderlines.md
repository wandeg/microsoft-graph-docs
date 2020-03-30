---
title: "Add salesOrderLines"
description: "Add salesOrderLines by posting to the salesOrderLines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesOrderLines

Namespace: microsoft.graph

Add salesOrderLines by posting to the salesOrderLines collection.

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
POST /financials/companies/{companyId}/salesOrderLines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [salesOrderLine](../resources/salesorderline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salesorderline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrderLines
Content-type: application/json
Content-length: 926

{
  "@odata.type": "#microsoft.graph.salesOrderLine",
  "documentId": "ad0679c0-79c0-ad06-c079-06adc07906ad",
  "sequence": 8,
  "itemId": "b63d2521-2521-b63d-2125-3db621253db6",
  "accountId": "93d19a1f-9a1f-93d1-1f9a-d1931f9ad193",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "e854acc8-acc8-e854-c8ac-54e8c8ac54e8",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.salesorderline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 975

{
  "@odata.type": "#microsoft.graph.salesOrderLine",
  "id": "b6617c4d-7c4d-b661-4d7c-61b64d7c61b6",
  "documentId": "ad0679c0-79c0-ad06-c079-06adc07906ad",
  "sequence": 8,
  "itemId": "b63d2521-2521-b63d-2125-3db621253db6",
  "accountId": "93d19a1f-9a1f-93d1-1f9a-d1931f9ad193",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "e854acc8-acc8-e854-c8ac-54e8c8ac54e8",
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

