---
title: "Create itemCategory"
description: "Create a new itemCategory object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create itemCategory

Namespace: microsoft.graph

Create a new [itemCategory](../resources/itemcategory.md) object.

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
POST /financials/companies/{companyId}/itemCategories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [itemCategory](../resources/itemcategory.md) object.

The following table shows the properties that are required when you create the [itemCategory](../resources/itemcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [itemCategory](../resources/itemcategory.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itemcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/itemCategories
Content-type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.itemCategory",
  "code": "Code value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.itemcategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.itemCategory",
  "id": "62710455-0455-6271-5504-716255047162",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
}
```

