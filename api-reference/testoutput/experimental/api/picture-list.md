---
title: "List pictures"
description: "List properties and relationships of the picture objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List pictures

Namespace: microsoft.graph

List properties and relationships of the [picture](../resources/picture.md) objects.

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
GET /financials/companies/{companyId}/picture
GET /financials/companies/{companyId}/items/{itemId}/picture
GET /financials/companies/{companyId}/vendors/{vendorId}/picture
GET /financials/companies/{companyId}/customers/{customerId}/picture
GET /financials/companies/{companyId}/employees/{employeeId}/picture
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [picture](../resources/picture.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_picture"
}
-->
``` http
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/picture
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.picture)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 250

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.picture",
      "id": "94a23027-3027-94a2-2730-a2942730a294",
      "width": 5,
      "height": 6,
      "contentType": "Content Type value",
      "content": "Stream"
    }
  ]
}
```

