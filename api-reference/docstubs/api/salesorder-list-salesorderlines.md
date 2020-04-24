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
GET /financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines
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
If successful, this method returns a `200 OK` response code and a collection of [salesOrderLine](../resources/salesorderline.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_salesorderline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/salesOrders/{salesOrderId}/salesOrderLines
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
      "id": "f35cc1de-c1de-f35c-dec1-5cf3dec15cf3",
      "documentId": "165821c2-21c2-1658-c221-5816c2215816",
      "sequence": 8,
      "itemId": "4443d486-d486-4443-86d4-434486d44344",
      "accountId": "157ed6fe-d6fe-157e-fed6-7e15fed67e15",
      "lineType": "Line Type value",
      "description": "Description value",
      "unitOfMeasureId": "d75c434a-434a-d75c-4a43-5cd74a435cd7",
      "quantity": "4.2",
      "unitPrice": "4.2",
      "discountAmount": "4.2",
      "discountPercent": "4.2",
      "discountAppliedBeforeTax": true,
      "amountExcludingTax": "4.2",
      "taxCode": "Tax Code value",
      "taxPercent": "4.2",
      "totalTaxAmount": "4.2",
      "amountIncludingTax": "4.2",
      "invoiceDiscountAllocation": "4.2",
      "netAmount": "4.2",
      "netTaxAmount": "4.2",
      "netAmountIncludingTax": "4.2",
      "shipmentDate": "Date",
      "shippedQuantity": "4.2",
      "invoicedQuantity": "4.2",
      "invoiceQuantity": "4.2",
      "shipQuantity": "4.2"
    }
  ]
}
```

