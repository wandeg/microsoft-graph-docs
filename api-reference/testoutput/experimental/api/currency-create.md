---
title: "Create currency"
description: "Create a new currency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create currency

Namespace: microsoft.graph

Create a new [currency](../resources/currency.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies/{companyId}/currencies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [currency](../resources/currency.md) object.

The following table shows the properties that are required when you create the [currency](../resources/currency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|symbol|String||
|amountDecimalPlaces|String||
|amountRoundingPrecision|Decimal||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [currency](../resources/currency.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_currency_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/currencies
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.currency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 351

{
  "@odata.type": "#microsoft.graph.currency",
  "id": "eb1de9a6-e9a6-eb1d-a6e9-1deba6e91deb",
  "code": "Code value",
  "displayName": "Display Name value",
  "symbol": "Symbol value",
  "amountDecimalPlaces": "Amount Decimal Places value",
  "amountRoundingPrecision": "4.2",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

