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

## HTTP request
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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [salesCreditMemo](../resources/salescreditmemo.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemo"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
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
    "id": "95018648-8648-9501-4886-019548860195",
    "number": "Number value",
    "externalDocumentNumber": "External Document Number value",
    "creditMemoDate": "Date",
    "dueDate": "Date",
    "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
    "customerNumber": "Customer Number value",
    "customerName": "Customer Name value",
    "billToName": "Bill To Name value",
    "billToCustomerId": "e072e734-e734-e072-34e7-72e034e772e0",
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
    "currencyId": "0727dad2-dad2-0727-d2da-2707d2da2707",
    "currencyCode": "Currency Code value",
    "paymentTermsId": "1470d31f-d31f-1470-1fd3-70141fd37014",
    "salesperson": "Salesperson value",
    "pricesIncludeTax": true,
    "discountAmount": "4.2",
    "discountAppliedBeforeTax": true,
    "totalAmountExcludingTax": "4.2",
    "totalTaxAmount": "4.2",
    "totalAmountIncludingTax": "4.2",
    "status": "Status value",
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00",
    "invoiceId": "64d5f2e7-f2e7-64d5-e7f2-d564e7f2d564",
    "invoiceNumber": "Invoice Number value",
    "phoneNumber": "Phone Number value",
    "email": "Email value"
  }
}
```

