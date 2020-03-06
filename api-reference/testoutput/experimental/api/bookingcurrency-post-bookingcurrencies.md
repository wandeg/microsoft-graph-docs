---
title: "Create bookingCurrency"
description: "Create a new bookingCurrency object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create bookingCurrency

Namespace: microsoft.graph

Create a new [bookingCurrency](../resources/bookingcurrency.md) object.

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
POST /bookingCurrencies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [bookingCurrency](../resources/bookingcurrency.md) object.

The following table shows the properties that are required when you create the [bookingCurrency](../resources/bookingcurrency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|symbol|String||



## Response
If successful, this method returns a `201 Created` response code and a [bookingCurrency](../resources/bookingcurrency.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_bookingcurrency_from_bookingcurrencies"
}
-->
``` http
POST https://graph.microsoft.com/localtest/bookingCurrencies
Content-type: application/json
Content-length: 86

{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "symbol": "Symbol value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingcurrency"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 135

{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "id": "ef5940b8-40b8-ef59-b840-59efb84059ef",
  "symbol": "Symbol value"
}
```

