---
title: "List customerPayments"
description: "Get the customerPayments from the customerPayments navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List customerPayments

Namespace: microsoft.graph

Get the customerPayments from the customerPayments navigation property.

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
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [customerPayment](../resources/customerpayment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customerpayment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.customerpayment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 836

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.customerPayment",
      "id": "898865e5-65e5-8988-e565-8889e5658889",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "customerId": "a61f8986-8986-a61f-8689-1fa686891fa6",
      "customerNumber": "Customer Number value",
      "contactId": "Contact Id value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "appliesToInvoiceId": "ca957a91-7a91-ca95-917a-95ca917a95ca",
      "appliesToInvoiceNumber": "Applies To Invoice Number value",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
    }
  ]
}
```

