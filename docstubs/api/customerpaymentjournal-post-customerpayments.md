---
title: "Add customerPayments"
description: "Add customerPayments by posting to the customerPayments collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add customerPayments

Namespace: microsoft.graph

Add customerPayments by posting to the customerPayments collection.

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
POST /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [customerPayment](../resources/customerpayment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_customerpayment_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments
Content-type: application/json
Content-length: 626

{
  "@odata.type": "#microsoft.graph.customerPayment",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
  "customerNumber": "Customer Number value",
  "contactId": "Contact Id value",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "externalDocumentNumber": "External Document Number value",
  "amount": "4.2",
  "appliesToInvoiceId": "94757752-7752-9475-5277-759452777594",
  "appliesToInvoiceNumber": "Applies To Invoice Number value",
  "description": "Description value",
  "comment": "Comment value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.customerpayment"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 739

{
  "@odata.type": "#microsoft.graph.customerPayment",
  "id": "574da87c-a87c-574d-7ca8-4d577ca84d57",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "customerId": "3992e4c5-e4c5-3992-c5e4-9239c5e49239",
  "customerNumber": "Customer Number value",
  "contactId": "Contact Id value",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "externalDocumentNumber": "External Document Number value",
  "amount": "4.2",
  "appliesToInvoiceId": "94757752-7752-9475-5277-759452777594",
  "appliesToInvoiceNumber": "Applies To Invoice Number value",
  "description": "Description value",
  "comment": "Comment value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```

