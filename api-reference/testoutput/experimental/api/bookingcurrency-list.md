---
title: "List bookingCurrencies"
description: "List properties and relationships of the bookingCurrency objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List bookingCurrencies

Namespace: microsoft.graph

List properties and relationships of the [bookingCurrency](../resources/bookingcurrency.md) objects.

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
GET /bookingCurrencies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [bookingCurrency](../resources/bookingcurrency.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_bookingcurrency"
}
-->
``` http
GET https://graph.microsoft.com/localtest/bookingCurrencies
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.bookingcurrency)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 180

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.bookingCurrency",
      "id": "7653a81e-a81e-7653-1ea8-53761ea85376",
      "symbol": "Symbol value"
    }
  ]
}
```

