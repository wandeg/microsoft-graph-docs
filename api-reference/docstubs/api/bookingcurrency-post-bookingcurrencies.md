---
title: "Create bookingCurrency"
description: "Create a new bookingCurrency object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create bookingCurrency

Namespace: microsoft.graph

Create a new [bookingCurrency](../resources/bookingcurrency.md) object.

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
POST /bookingCurrencies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [bookingCurrency](../resources/bookingcurrency.md) object.

The following table shows the properties that are required when you create the [bookingCurrency](../resources/bookingcurrency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|symbol|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [bookingCurrency](../resources/bookingcurrency.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_bookingcurrency_from_bookingcurrencies"
}
-->
``` http
POST https://graph.microsoft.com/beta/bookingCurrencies
Content-Type: application/json
Content-length: 86

{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "symbol": "Symbol value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingcurrency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "id": "87d7f032-f032-87d7-32f0-d78732f0d787",
  "symbol": "Symbol value"
}
```

