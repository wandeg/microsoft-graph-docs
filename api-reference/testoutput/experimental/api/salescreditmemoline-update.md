---
title: "Update salesCreditMemoLine"
description: "Update the properties of a salesCreditMemoLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesCreditMemoLine

Namespace: microsoft.graph

Update the properties of a [salesCreditMemoLine](../resources/salescreditmemoline.md) object.

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
PATCH /financials/companies/{companyId}/salesCreditMemoLines/{salesCreditMemoLineId}
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [salesCreditMemoLine](../resources/salescreditmemoline.md) object.

The following table shows the properties that are required when you create the [salesCreditMemoLine](../resources/salescreditmemoline.md).

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
|unitPrice|Decimal||
|quantity|Decimal||
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



## Response
If successful, this method returns a `200 OK` response code and an updated [salesCreditMemoLine](../resources/salescreditmemoline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salescreditmemoline"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesCreditMemoLines/{salesCreditMemoLineId}
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.salesCreditMemoLine",
  "documentId": "f25796de-96de-f257-de96-57f2de9657f2",
  "sequence": 8,
  "itemId": "39a5aaf7-aaf7-39a5-f7aa-a539f7aaa539",
  "accountId": "16975858-5858-1697-5858-971658589716",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "8736d1fa-d1fa-8736-fad1-3687fad13687",
  "unitPrice": "4.2",
  "quantity": "4.2",
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
  "shipmentDate": "Date"
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
Content-Length: 866

{
  "@odata.type": "#microsoft.graph.salesCreditMemoLine",
  "id": "a673ef25-ef25-a673-25ef-73a625ef73a6",
  "documentId": "f25796de-96de-f257-de96-57f2de9657f2",
  "sequence": 8,
  "itemId": "39a5aaf7-aaf7-39a5-f7aa-a539f7aaa539",
  "accountId": "16975858-5858-1697-5858-971658589716",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "8736d1fa-d1fa-8736-fad1-3687fad13687",
  "unitPrice": "4.2",
  "quantity": "4.2",
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
  "shipmentDate": "Date"
}
```

