---
title: "Get account"
description: "Read properties and relationships of the account object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get account

Namespace: microsoft.graph

Read properties and relationships of the [account](../resources/account.md) object.

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
GET /financials/companies/{companyId}/accounts/{accountId}
GET /financials/companies/{companyId}/journals/{journalId}/account
GET /financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}/account
GET /financials/companies/{companyId}/journals/{journalId}/journalLines/{journalLineId}/account
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/account
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}/account
GET /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}/account
GET /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/{salesInvoiceLineId}/account
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}/account
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/purchaseInvoiceLines/{purchaseInvoiceLineId}/account
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
If successful, this method returns a `200 OK` response code and [account](../resources/account.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_account"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/accounts/{accountId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.account"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
    "@odata.type": "#microsoft.graph.account",
    "id": "372f761d-761d-372f-1d76-2f371d762f37",
    "number": "Number value",
    "displayName": "Display Name value",
    "category": "Category value",
    "subCategory": "Sub Category value",
    "blocked": true,
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00"
  }
}
```

