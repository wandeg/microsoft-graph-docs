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
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [customerPayment](../resources/customerpayment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_customerpayment"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments
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
      "id": "40bf12a9-12a9-40bf-a912-bf40a912bf40",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "customerId": "8f5f13a0-13a0-8f5f-a013-5f8fa0135f8f",
      "customerNumber": "Customer Number value",
      "contactId": "Contact Id value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "appliesToInvoiceId": "cf0f1428-1428-cf0f-2814-0fcf28140fcf",
      "appliesToInvoiceNumber": "Applies To Invoice Number value",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00"
    }
  ]
}
```

