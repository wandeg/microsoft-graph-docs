---
title: "Get salesCreditMemoLine"
description: "Read properties and relationships of the salesCreditMemoLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesCreditMemoLine

Namespace: microsoft.graph

Read properties and relationships of the [salesCreditMemoLine](../resources/salescreditmemoline.md) object.

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
GET /financials/companies/{companyId}/salesCreditMemoLines/{salesCreditMemoLineId}
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}
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
If successful, this method returns a `200 OK` response code and [salesCreditMemoLine](../resources/salescreditmemoline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemoline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemoLines/{salesCreditMemoLineId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesCreditMemoLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 933

{
  "value": {
    "@odata.type": "#microsoft.graph.salesCreditMemoLine",
    "id": "4f7b455f-455f-4f7b-5f45-7b4f5f457b4f",
    "documentId": "281b957c-957c-281b-7c95-1b287c951b28",
    "sequence": 8,
    "itemId": "59773775-3775-5977-7537-775975377759",
    "accountId": "9b2499a0-99a0-9b24-a099-249ba099249b",
    "lineType": "Line Type value",
    "description": "Description value",
    "unitOfMeasureId": "0efb44f6-44f6-0efb-f644-fb0ef644fb0e",
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
}
```

