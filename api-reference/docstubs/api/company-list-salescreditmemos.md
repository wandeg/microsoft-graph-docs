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
Content-Length: 1764

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesCreditMemo",
      "id": "1001e451-e451-1001-51e4-011051e40110",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "creditMemoDate": "Date",
      "dueDate": "Date",
      "customerId": "96a89bff-9bff-96a8-ff9b-a896ff9ba896",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "9b1f7785-7785-9b1f-8577-1f9b85771f9b",
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
      "currencyId": "93b64d88-4d88-93b6-884d-b693884db693",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "8173a089-a089-8173-89a0-738189a07381",
      "salesperson": "Salesperson value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:59:12.2914176+03:00",
      "invoiceId": "e7762ad6-2ad6-e776-d62a-76e7d62a76e7",
      "invoiceNumber": "Invoice Number value",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

