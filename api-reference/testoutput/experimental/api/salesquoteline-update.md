---
title: "Update salesQuoteLine"
description: "Update the properties of a salesQuoteLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update salesQuoteLine

Namespace: microsoft.graph

Update the properties of a [salesQuoteLine](../resources/salesquoteline.md) object.

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
PATCH /financials/companies/{companyId}/salesQuoteLines/{salesQuoteLineId}
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [salesQuoteLine](../resources/salesquoteline.md) object.

The following table shows the properties that are required when you create the [salesQuoteLine](../resources/salesquoteline.md).

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
|netAmount|Decimal||
|netTaxAmount|Decimal||
|netAmountIncludingTax|Decimal||



## Response
If successful, this method returns a `200 OK` response code and an updated [salesQuoteLine](../resources/salesquoteline.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_salesquoteline"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesQuoteLines/{salesQuoteLineId}
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "documentId": "a4d6f8da-f8da-a4d6-daf8-d6a4daf8d6a4",
  "sequence": 8,
  "itemId": "d76ea287-a287-d76e-87a2-6ed787a26ed7",
  "accountId": "95554513-4513-9555-1345-559513455595",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "c915dcf5-dcf5-c915-f5dc-15c9f5dc15c9",
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
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2"
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
Content-Length: 795

{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "id": "79aec911-c911-79ae-11c9-ae7911c9ae79",
  "documentId": "a4d6f8da-f8da-a4d6-daf8-d6a4daf8d6a4",
  "sequence": 8,
  "itemId": "d76ea287-a287-d76e-87a2-6ed787a26ed7",
  "accountId": "95554513-4513-9555-1345-559513455595",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "c915dcf5-dcf5-c915-f5dc-15c9f5dc15c9",
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
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2"
}
```

