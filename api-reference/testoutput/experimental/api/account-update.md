---
title: "Update account"
description: "Update the properties of a account object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update account

Namespace: microsoft.graph

Update the properties of a [account](../resources/account.md) object.

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
PATCH /financials/companies/{companyId}/accounts/{accountId}
PATCH /financials/companies/{companyId}/journals/{journalId}/account
PATCH /financials/companies/{companyId}/generalLedgerEntries/{generalLedgerEntryId}/account
PATCH /financials/companies/{companyId}/journals/{journalId}/journalLines/{journalLineId}/account
PATCH /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/account
PATCH /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines/{salesOrderLineId}/account
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/salesQuoteLines/{salesQuoteLineId}/account
PATCH /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines/{salesInvoiceLineId}/account
PATCH /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/salesCreditMemoLines/{salesCreditMemoLineId}/account
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/purchaseInvoiceLines/{purchaseInvoiceLineId}/account
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [account](../resources/account.md) object.

The following table shows the properties that are required when you create the [account](../resources/account.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|number|String||
|displayName|String||
|category|String||
|subCategory|String||
|blocked|Boolean||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [account](../resources/account.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_account"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/financials/companies/{companyId}/accounts/{accountId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.account",
  "number": "Number value",
  "displayName": "Display Name value",
  "category": "Category value",
  "subCategory": "Sub Category value",
  "blocked": true
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 324

{
  "@odata.type": "#microsoft.graph.account",
  "id": "180f96b3-96b3-180f-b396-0f18b3960f18",
  "number": "Number value",
  "displayName": "Display Name value",
  "category": "Category value",
  "subCategory": "Sub Category value",
  "blocked": true,
  "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
}
```

