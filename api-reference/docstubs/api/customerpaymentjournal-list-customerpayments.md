---
title: "List customerPayments"
description: "Get the customerPayments from the customerPayments navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List customerPayments

Namespace: microsoft.graph

Get the customerPayments from the customerPayments navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [customerPayment](../resources/customerpayment.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_customerpayment"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.customerpayment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.customerPayment",
      "id": "3544b47f-b47f-3544-7fb4-44357fb44435",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
      "customerNumber": "Customer Number value",
      "contactId": "Contact Id value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "appliesToInvoiceId": "6070022a-022a-6070-2a02-70602a027060",
      "appliesToInvoiceNumber": "Applies To Invoice Number value",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
    }
  ]
}
```

