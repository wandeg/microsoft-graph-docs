---
title: "Get salesCreditMemo"
description: "Read properties and relationships of the salesCreditMemo object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get salesCreditMemo

Namespace: microsoft.graph

Read properties and relationships of the [salesCreditMemo](../resources/salescreditmemo.md) object.

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
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
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
If successful, this method returns a `200 OK` response code and [salesCreditMemo](../resources/salescreditmemo.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemo"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesCreditMemo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1672

{
  "value": {
    "@odata.type": "#microsoft.graph.salesCreditMemo",
    "id": "699cbd1d-bd1d-699c-1dbd-9c691dbd9c69",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "creditMemoDate": "Date",
    "dueDate": "Date",
    "customerId": "a61f8986-8986-a61f-8689-1fa686891fa6",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "7a1538dc-38dc-7a15-dc38-157adc38157a",
    "billToCustomerNumber": "Bill To Customer Number value",
    "sellingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType",
      "street": "Street value",
      "city": "City value",
      "state": "State value",
      "countryLetterCode": "Country Letter Code value",
      "postalCode": "Postal Code value"
    },
    "billingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "currencyId": "5323df69-df69-5323-69df-235369df2353",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "292944c5-44c5-2929-c544-2929c5442929",
    "salesperson": "Salesperson value",
    "pricesIncludeTax": true,
    "discountAmount": "4.2",
    "discountAppliedBeforeTax": true,
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
    "invoiceId": "26c18131-8131-26c1-3181-c1263181c126",
    "invoiceNumber": "Invoice Number value",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

