---
title: "List salesOrderLines"
description: "Get the salesOrderLines from the salesOrderLines navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List salesOrderLines

Namespace: microsoft.graph

Get the salesOrderLines from the salesOrderLines navigation property.

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
GET /financials/companies/{companyId}/salesOrderLines
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

If successful, this method returns a `200 OK` response code and a collection of [salesOrderLine](../resources/salesorderline.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salesorderline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrderLines
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.salesorderline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.salesOrderLine",
      "id": "5c2d8e60-8e60-5c2d-608e-2d5c608e2d5c",
      "documentId": "Guid",
      "sequence": "Integer",
      "itemId": "Guid",
      "accountId": "Guid",
      "lineType": "String",
      "description": "String",
      "unitOfMeasureId": "Guid",
      "quantity": "Decimal",
      "unitPrice": "Decimal",
      "discountAmount": "Decimal",
      "discountPercent": "Decimal",
      "discountAppliedBeforeTax": "Boolean",
      "amountExcludingTax": "Decimal",
      "taxCode": "String",
      "taxPercent": "Decimal",
      "totalTaxAmount": "Decimal",
      "amountIncludingTax": "Decimal",
      "invoiceDiscountAllocation": "Decimal",
      "netAmount": "Decimal",
      "netTaxAmount": "Decimal",
      "netAmountIncludingTax": "Decimal",
      "shipmentDate": "Date",
      "shippedQuantity": "Decimal",
      "invoicedQuantity": "Decimal",
      "invoiceQuantity": "Decimal",
      "shipQuantity": "Decimal"
    }
  ]
}
```

