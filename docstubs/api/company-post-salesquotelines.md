---
title: "Add salesQuoteLines"
description: "Add salesQuoteLines by posting to the salesQuoteLines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add salesQuoteLines

Namespace: microsoft.graph

Add salesQuoteLines by posting to the salesQuoteLines collection.

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
POST /financials/companies/{companyId}/salesQuoteLines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [salesQuoteLine](../resources/salesquoteline.md) object.

The following table shows the properties that are required when you create the [salesQuoteLine](../resources/salesquoteline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|documentId|Guid||
|sequence|Int32||
|itemId|Guid||
|accountId|Guid||
|lineType|String||
|description|String||
|unitOfMeasureId|Guid||
|unitPrice|Decimal||
|quantity|Decimal||
|discountAmount|Decimal||
|discountPercent|Decimal||
|discountAppliedBeforeTax|Boolean||
|amountExcludingTax|Decimal||
|taxCode|String||
|taxPercent|Decimal||
|totalTaxAmount|Decimal||
|amountIncludingTax|Decimal||
|netAmount|Decimal||
|netTaxAmount|Decimal||
|netAmountIncludingTax|Decimal||



## Response
If successful, this method returns a `201 Created` response code and a [salesQuoteLine](../resources/salesquoteline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_salesquoteline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuoteLines
Content-type: application/json
Content-length: 746

{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "documentId": "2cd4c5df-c5df-2cd4-dfc5-d42cdfc5d42c",
  "sequence": 8,
  "itemId": "38e36916-6916-38e3-1669-e3381669e338",
  "accountId": "7085e644-e644-7085-44e6-857044e68570",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "af6b7225-7225-af6b-2572-6baf25726baf",
  "unitPrice": "4.2",
  "quantity": "4.2",
  "discountAmount": "4.2",
  "discountPercent": "4.2",
  "discountAppliedBeforeTax": true,
  "amountExcludingTax": "4.2",
  "taxCode": "Tax Code value",
  "taxPercent": "4.2",
  "totalTaxAmount": "4.2",
  "amountIncludingTax": "4.2",
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesquoteline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 795

{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "id": "e691d305-d305-e691-05d3-91e605d391e6",
  "documentId": "2cd4c5df-c5df-2cd4-dfc5-d42cdfc5d42c",
  "sequence": 8,
  "itemId": "38e36916-6916-38e3-1669-e3381669e338",
  "accountId": "7085e644-e644-7085-44e6-857044e68570",
  "lineType": "Line Type value",
  "description": "Description value",
  "unitOfMeasureId": "af6b7225-7225-af6b-2572-6baf25726baf",
  "unitPrice": "4.2",
  "quantity": "4.2",
  "discountAmount": "4.2",
  "discountPercent": "4.2",
  "discountAppliedBeforeTax": true,
  "amountExcludingTax": "4.2",
  "taxCode": "Tax Code value",
  "taxPercent": "4.2",
  "totalTaxAmount": "4.2",
  "amountIncludingTax": "4.2",
  "netAmount": "4.2",
  "netTaxAmount": "4.2",
  "netAmountIncludingTax": "4.2"
}
```

