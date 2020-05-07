---
title: "Get salesCreditMemo"
description: "Read the properties and relationships of a salesCreditMemo object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get salesCreditMemo

Namespace: microsoft.graph

Read the properties and relationships of a [salesCreditMemo](../resources/salescreditmemo.md) object.

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
GET /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [salesCreditMemo](../resources/salescreditmemo.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salescreditmemo"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesCreditMemo"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.salesCreditMemo",
    "id": "c66e47df-47df-c66e-df47-6ec6df476ec6",
    "number": "String",
    "externalDocumentNumber": "String",
    "creditMemoDate": "Date",
    "dueDate": "Date",
    "customerId": "Guid",
    "customerNumber": "String",
    "customerName": "String",
    "billToName": "String",
    "billToCustomerId": "Guid",
    "billToCustomerNumber": "String",
    "sellingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "billingPostalAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "currencyId": "Guid",
    "currencyCode": "String",
    "paymentTermsId": "Guid",
    "salesperson": "String",
    "pricesIncludeTax": "Boolean",
    "discountAmount": "Decimal",
    "discountAppliedBeforeTax": "Boolean",
    "totalAmountExcludingTax": "Decimal",
    "totalTaxAmount": "Decimal",
    "totalAmountIncludingTax": "Decimal",
    "status": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "invoiceId": "Guid",
    "invoiceNumber": "String",
    "phoneNumber": "String",
    "email": "String"
  }
}
```

