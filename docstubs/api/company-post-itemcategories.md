---
title: "Add itemCategories"
description: "Add itemCategories by posting to the itemCategories collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add itemCategories

Namespace: microsoft.graph

Add itemCategories by posting to the itemCategories collection.

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
POST /financials/companies/{companyId}/itemCategories/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_itemcategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/itemCategories
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
  "id": "99c44331-4331-99c4-3143-c4993143c499",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
}
```

