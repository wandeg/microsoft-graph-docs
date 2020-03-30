---
title: "Get itemCategory"
description: "Read properties and relationships of the itemCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get itemCategory

Namespace: microsoft.graph

Read properties and relationships of the [itemCategory](../resources/itemcategory.md) object.

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
GET /financials/companies/{companyId}/items/{itemId}/itemCategory
GET /financials/companies/{companyId}/itemCategories/{itemCategoryId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [itemCategory](../resources/itemcategory.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_itemcategory"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/items/{itemId}/itemCategory
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemCategory"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 261

{
  "value": {
    "@odata.type": "#microsoft.graph.itemCategory",
    "id": "17f0ab88-ab88-17f0-88ab-f01788abf017",
    "code": "Code value",
    "displayName": "Display Name value",
    "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00"
  }
}
```

