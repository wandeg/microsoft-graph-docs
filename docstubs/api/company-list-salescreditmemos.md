---
title: "List salesCreditMemos"
description: "Get the salesCreditMemos from the salesCreditMemos navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List salesCreditMemos

Namespace: microsoft.graph

Get the salesCreditMemos from the salesCreditMemos navigation property.

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
GET /financials/companies/{companyId}/salesCreditMemos
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
If successful, this method returns a `200 OK` response code and a collection of [salesCreditMemo](../resources/salescreditmemo.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemo"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salescreditmemo)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1763

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesCreditMemo",
      "id": "8483a3b8-a3b8-8483-b8a3-8384b8a38384",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "creditMemoDate": "Date",
      "dueDate": "Date",
      "customerId": "8abcd51d-d51d-8abc-1dd5-bc8a1dd5bc8a",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "fee1cc02-cc02-fee1-02cc-e1fe02cce1fe",
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
      "currencyId": "d358c210-c210-d358-10c2-58d310c258d3",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "2b1121b8-21b8-2b11-b821-112bb821112b",
      "salesperson": "Salesperson value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2017-01-01T00:02:23.471109+03:00",
      "invoiceId": "66f8b74b-b74b-66f8-4bb7-f8664bb7f866",
      "invoiceNumber": "Invoice Number value",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

