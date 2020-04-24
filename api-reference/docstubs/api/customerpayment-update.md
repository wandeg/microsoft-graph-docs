---
title: "Update customerPayment"
description: "Update the properties of a customerPayment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update customerPayment

Namespace: microsoft.graph

Update the properties of a [customerPayment](../resources/customerpayment.md) object.

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
PATCH /financials/companies/{companyId}/customerPayments/{customerPaymentId}
PATCH /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [customerPayment](../resources/customerpayment.md) object.

The following table shows the properties that are required when you create the [customerPayment](../resources/customerpayment.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String|**TODO: Add Description**|
|lineNumber|Int32|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|customerNumber|String|**TODO: Add Description**|
|contactId|String|**TODO: Add Description**|
|postingDate|Date|**TODO: Add Description**|
|documentNumber|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|amount|Decimal|**TODO: Add Description**|
|appliesToInvoiceId|Guid|**TODO: Add Description**|
|appliesToInvoiceNumber|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|comment|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [customerPayment](../resources/customerpayment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_customerpayment"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/customerPayments/{customerPaymentId}
Content-Type: application/json
Content-length: 626

{
  "@odata.type": "#microsoft.graph.customerPayment",
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
  "comment": "Comment value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
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
```

