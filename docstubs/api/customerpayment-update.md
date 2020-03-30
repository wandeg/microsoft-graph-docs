---
title: "Update customerPayment"
description: "Update the properties of a customerPayment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update customerPayment

Namespace: microsoft.graph

Update the properties of a [customerPayment](../resources/customerpayment.md) object.

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
PATCH /financials/companies/{companyId}/customerPayments/{customerPaymentId}
PATCH /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [customerPayment](../resources/customerpayment.md) object.

The following table shows the properties that are required when you create the [customerPayment](../resources/customerpayment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String||
|lineNumber|Int32||
|customerId|Guid||
|customerNumber|String||
|contactId|String||
|postingDate|Date||
|documentNumber|String||
|externalDocumentNumber|String||
|amount|Decimal||
|appliesToInvoiceId|Guid||
|appliesToInvoiceNumber|String||
|description|String||
|comment|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [customerPayment](../resources/customerpayment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_customerpayment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPayments/{customerPaymentId}
Content-type: application/json
Content-length: 626

{
  "@odata.type": "#microsoft.graph.customerPayment",
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
  "comment": "Comment value"
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
Content-Length: 739

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
```

