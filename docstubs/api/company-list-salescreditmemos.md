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
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemo"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "5ac8117b-117b-5ac8-7b11-c85a7b11c85a",
      "number": "Number value",
      "externalDocumentNumber": "External Document Number value",
      "creditMemoDate": "Date",
      "dueDate": "Date",
      "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
      "customerNumber": "Customer Number value",
      "customerName": "Customer Name value",
      "billToName": "Bill To Name value",
      "billToCustomerId": "9e27a69a-a69a-9e27-9aa6-279e9aa6279e",
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
      "currencyId": "83ed47d1-47d1-83ed-d147-ed83d147ed83",
      "currencyCode": "Currency Code value",
      "paymentTermsId": "be513a4b-3a4b-be51-4b3a-51be4b3a51be",
      "salesperson": "Salesperson value",
      "pricesIncludeTax": true,
      "discountAmount": "4.2",
      "discountAppliedBeforeTax": true,
      "totalAmountExcludingTax": "4.2",
      "totalTaxAmount": "4.2",
      "totalAmountIncludingTax": "4.2",
      "status": "Status value",
      "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00",
      "invoiceId": "7ab106de-06de-7ab1-de06-b17ade06b17a",
      "invoiceNumber": "Invoice Number value",
      "phoneNumber": "Phone Number value",
      "email": "Email value"
    }
  ]
}
```

