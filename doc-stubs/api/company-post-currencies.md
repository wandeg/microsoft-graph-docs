---
title: "Create currencies"
description: "Create a new currencies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create currencies

Namespace: microsoft.graph

Create a new currencies object.

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
POST /financials/companies/{companyId}/currencies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `201 Created` response code and a [currency](../resources/currency.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_currency_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/currencies
Content-Type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.currency",
  "code": "String",
  "displayName": "String",
  "symbol": "String",
  "amountDecimalPlaces": "String",
  "amountRoundingPrecision": "Decimal"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.currency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.currency",
  "id": "edbd813b-813b-edbd-3b81-bded3b81bded",
  "code": "String",
  "displayName": "String",
  "symbol": "String",
  "amountDecimalPlaces": "String",
  "amountRoundingPrecision": "Decimal",
  "lastModifiedDateTime": "String (timestamp)"
}
```

