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
|Name|Description|
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
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemoLines/{salesCreditMemoLineId}
Content-type: application/json
Content-length: 817

{
  "@odata.type": "#microsoft.graph.salesCreditMemoLine",
  "documentId": "5bfe0542-0542-5bfe-4205-fe5b4205fe5b",
  "sequence": 8,
  "itemId": "33ceb353-b353-33ce-53b3-ce3353b3ce33",
  "accountId": "ec2602f3-02f3-ec26-f302-26ecf30226ec",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "dfeb54c9-54c9-dfeb-c954-ebdfc954ebdf",
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
  "id": "bddf7c05-7c05-bddf-057c-dfbd057cdfbd",
  "documentId": "5bfe0542-0542-5bfe-4205-fe5b4205fe5b",
  "sequence": 8,
  "itemId": "33ceb353-b353-33ce-53b3-ce3353b3ce33",
  "accountId": "ec2602f3-02f3-ec26-f302-26ecf30226ec",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "dfeb54c9-54c9-dfeb-c954-ebdfc954ebdf",
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

