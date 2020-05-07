---
title: "Update picture"
description: "Update the properties of a picture object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update picture

Namespace: microsoft.graph

Update the properties of a picture object.

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
PATCH /financials/companies/{companyId}/vendors/{vendorId}/picture
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [picture](../resources/picture.md) object.

The following table shows the properties that are required when you create the [picture](../resources/picture.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|width|Int32|**TODO: Add Description**|
|height|Int32|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|content|Stream|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [picture](../resources/picture.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_picture"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/vendors/{vendorId}/picture
Content-Type: application/json
Content-length: 148

{
  "@odata.type": "#microsoft.graph.picture",
  "width": "Integer",
  "height": "Integer",
  "contentType": "String",
  "content": "Stream"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.picture",
  "id": "b67bb47a-b47a-b67b-7ab4-7bb67ab47bb6",
  "width": "Integer",
  "height": "Integer",
  "contentType": "String",
  "content": "Stream"
}
```

