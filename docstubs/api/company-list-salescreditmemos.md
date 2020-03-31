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
      "id": "3652b113-b113-3652-13b1-523613b15236",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "creditMemoDate": "Date",
      "dueDate": "Date",
      "customerId": "b5483775-3775-b548-7537-48b5753748b5",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "cae7ad11-ad11-cae7-11ad-e7ca11ade7ca",
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
      "currencyId": "2ff7fc3c-fc3c-2ff7-3cfc-f72f3cfcf72f",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "c9d77067-7067-c9d7-6770-d7c96770d7c9",
      "salesperson": "Salesperson value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00",
      "invoiceId": "9eac7b80-7b80-9eac-807b-ac9e807bac9e",
      "invoiceNumber": "Invoice Number value",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

