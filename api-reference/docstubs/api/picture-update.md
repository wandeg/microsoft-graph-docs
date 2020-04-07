---
title: "Update picture"
description: "Update the properties of a picture object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update picture

Namespace: microsoft.graph

Update the properties of a [picture](../resources/picture.md) object.

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
PATCH /financials/companies/{companyId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/items/{itemId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/vendors/{vendorId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/customers/{customerId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/employees/{employeeId}/picture/{pictureId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [picture](../resources/picture.md) object.

The following table shows the properties that are required when you create the [picture](../resources/picture.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|width|Int32||
|height|Int32||
|contentType|String||
|content|Stream||



## Response
If successful, this method returns a `200 OK` response code and an updated [picture](../resources/picture.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_picture"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/picture/{pictureId}
Content-type: application/json
Content-length: 144

{
  "@odata.type": "#microsoft.graph.picture",
  "width": 5,
  "height": 6,
  "contentType": "Content Type value",
  "content": "Stream"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 193

{
  "@odata.type": "#microsoft.graph.picture",
  "id": "c17bb53e-b53e-c17b-3eb5-7bc13eb57bc1",
  "width": 5,
  "height": 6,
  "contentType": "Content Type value",
  "content": "Stream"
}
```

