---
title: "Create columnLinks"
description: "Create a new columnLinks object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create columnLinks

Namespace: microsoft.graph

Create a new columnLinks object.

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
POST /drives/{drivesId}/list/contentTypes/{contentTypeId}/columnLinks
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [columnLink](../resources/columnlink.md) object.

The following table shows the properties that are required when you create the [columnLink](../resources/columnlink.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|name|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [columnLink](../resources/columnlink.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_columnlink_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/drives/{drivesId}/list/contentTypes/{contentTypeId}/columnLinks
Content-Type: application/json
Content-length: 73

{
  "@odata.type": "#microsoft.graph.columnLink",
  "name": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.columnlink"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.columnLink",
  "id": "f2c90d6e-0d6e-f2c9-6e0d-c9f26e0dc9f2",
  "name": "String"
}
```

