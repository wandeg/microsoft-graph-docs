---
title: "Create salesQuoteLines"
description: "Create a new salesQuoteLines object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesQuoteLines

Namespace: microsoft.graph

Create a new salesQuoteLines object.

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
POST /financials/companies/{companyId}/salesQuoteLines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [salesQuoteLine](../resources/salesquoteline.md) object.

The following table shows the properties that are required when you create the [salesQuoteLine](../resources/salesquoteline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|documentId|Guid|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|itemId|Guid|**TODO: Add Description**|
|accountId|Guid|**TODO: Add Description**|
|lineType|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|unitOfMeasureId|Guid|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|
|quantity|Decimal|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|amountExcludingTax|Decimal|**TODO: Add Description**|
|taxCode|String|**TODO: Add Description**|
|taxPercent|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|amountIncludingTax|Decimal|**TODO: Add Description**|
|netAmount|Decimal|**TODO: Add Description**|
|netTaxAmount|Decimal|**TODO: Add Description**|
|netAmountIncludingTax|Decimal|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [salesQuoteLine](../resources/salesquoteline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salesquoteline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuoteLines
Content-Type: application/json
Content-length: 647

{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "documentId": "Guid",
  "sequence": "Integer",
  "itemId": "Guid",
  "accountId": "Guid",
  "lineType": "String",
  "description": "String",
  "unitOfMeasureId": "Guid",
  "unitPrice": "Decimal",
  "quantity": "Decimal",
  "discountAmount": "Decimal",
  "discountPercent": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "amountExcludingTax": "Decimal",
  "taxCode": "String",
  "taxPercent": "Decimal",
  "totalTaxAmount": "Decimal",
  "amountIncludingTax": "Decimal",
  "netAmount": "Decimal",
  "netTaxAmount": "Decimal",
  "netAmountIncludingTax": "Decimal"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesquoteline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "id": "90d7ea88-ea88-90d7-88ea-d79088ead790",
  "documentId": "Guid",
  "sequence": "Integer",
  "itemId": "Guid",
  "accountId": "Guid",
  "lineType": "String",
  "description": "String",
  "unitOfMeasureId": "Guid",
  "unitPrice": "Decimal",
  "quantity": "Decimal",
  "discountAmount": "Decimal",
  "discountPercent": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "amountExcludingTax": "Decimal",
  "taxCode": "String",
  "taxPercent": "Decimal",
  "totalTaxAmount": "Decimal",
  "amountIncludingTax": "Decimal",
  "netAmount": "Decimal",
  "netTaxAmount": "Decimal",
  "netAmountIncludingTax": "Decimal"
}
```

