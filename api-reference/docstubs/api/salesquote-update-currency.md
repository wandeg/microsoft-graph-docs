---
title: "Update currency"
description: "Update the properties of a currency object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update currency

Namespace: microsoft.graph

Update the properties of a currency object.

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
PATCH /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/currency
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [currency](../resources/currency.md) object.

The following table shows the properties that are required when you create the [currency](../resources/currency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|symbol|String|**TODO: Add Description**|
|amountDecimalPlaces|String|**TODO: Add Description**|
|amountRoundingPrecision|Decimal|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [currency](../resources/currency.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_currency"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/salesQuotes/{salesQuoteId}/currency
Content-Type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.currency",
  "code": "Code value",
  "displayName": "Display Name value",
  "symbol": "Symbol value",
  "amountDecimalPlaces": "Amount Decimal Places value",
  "amountRoundingPrecision": "4.2"
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
  "@odata.type": "#microsoft.graph.currency",
  "id": "ead59cda-9cda-ead5-da9c-d5eada9cd5ea",
  "code": "Code value",
  "displayName": "Display Name value",
  "symbol": "Symbol value",
  "amountDecimalPlaces": "Amount Decimal Places value",
  "amountRoundingPrecision": "4.2",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```

