---
title: "Get customerPayment"
description: "Read properties and relationships of the customerPayment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get customerPayment

Namespace: microsoft.graph

Read properties and relationships of the [customerPayment](../resources/customerpayment.md) object.

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
GET /financials/companies/{companyId}/customerPayments/{customerPaymentId}
GET /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}
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
If successful, this method returns a `200 OK` response code and [customerPayment](../resources/customerpayment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customerpayment"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPayments/{customerPaymentId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customerPayment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 790

{
  "value": {
    "@odata.type": "#microsoft.graph.customerPayment",
    "id": "1ea04a00-4a00-1ea0-004a-a01e004aa01e",
    "journalDisplayName": "Journal Display Name value",
    "lineNumber": 10,
    "customerId": "b5483775-3775-b548-7537-48b5753748b5",
    "customerNumber": "Customer Number value",
    "contactId": "Contact Id value",
    "postingDate": "Date",
    "documentNumber": "Document Number value",
    "externalDocumentNumber": "External Document Number value",
    "amount": "4.2",
    "appliesToInvoiceId": "0dcd8e19-8e19-0dcd-198e-cd0d198ecd0d",
    "appliesToInvoiceNumber": "Applies To Invoice Number value",
    "description": "Description value",
    "comment": "Comment value",
    "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
  }
}
```

